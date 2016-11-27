---
title: "ImprovingModMono"
lastmodified: '2008-06-25'
redirect_from:
  - /ImprovingModMono/
---

ImprovingModMono
================

The following are suggestions on things that we could do to improve mod_mono:

From Joshua Tauberer:

-   Program output (stdout/stderr) should be redirected to something other than the main server error log (root access only). Maybe viewable in the control panel.

-   Afair, there are pairs of commands that do the same thing (MonoApplications, AddMonoApplications), which is confusing.

-   The examples on the wiki use Alias, and I never understood why that was necessary. That has always confused me.

-   Failures in the module that yield 500/503s should always send debugging info somewhere, and it should send it to somewhere that you don't need root access to view. It might also be a good idea to override the default response page to include the underlying error that occurred and suggested fixes.

-   It should be possible to have autoconfiguration work and use either A) one process for all vhosts or B) a different process for each vhost. And, it shouldn't be necessary to turn off autoconfiguration to get vhosts to work on their own process.

-   The notion of a server alias is not clear whether it has scope within a vhost or across vhosts.

-   I don't think MonoMaxMemory, MonoMaxCPUTime work (last I tried it).

-   Easier selection of the 1.0 vs 2.0 runtime.

From Ted Milker:

When MonoDebug is present in apache's configuration file, true or false, it spams up the apache error log with:

    [Fri May 04 08:33:20 2007] [error] Not running mod-mono-server.exe
    because no MonoApplications, MonoApplicationsConfigFile or
    MonoApplicationConfigDir specified.

If you remove MonoDebug, this message goes away. There is some behavior in mod_mono that does something different when MonoDebug is present(even if set to false) that probably needs to be looked at.

Regarding the many instances of mod-mono-server that are spawned when Apache's MPM==prefork Apache launches many mod-mono-servers, only one of them survives. This is due to limits in the APR locking interfaces. If newer versions of APR support better locking interfaces, we should take advantage of those. [I have a patch in the works for this that doesn't use locking at all (surprisingly). -JT]

