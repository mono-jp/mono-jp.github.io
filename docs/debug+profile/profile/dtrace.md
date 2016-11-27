---
title: DTrace
redirect_from:
  - /DTrace/
---

Using DTrace with Mono
----------------------

Mono 2.0 includes DTrace probes when configured with `--enable-dtrace`. This currently works on Solaris 10, OpenSolaris and Mac OS X v10.5.

The idea behind DTrace is that production copies of software are traceable in case problems arise, without needing to compile a debug version first. Both the kernel and many daemons or applications allow tracing in a scripted, event-oriented way.

You can use DTrace from the dtrace command line tool, graphically from OpenSolaris' Chime or Apple's Instruments and from various scripting languages.

To check if DTrace is enabled in your copy of Mono, run the following command:

``` bash
 $ dtrace -P mono'$target' -l -c mono
```

This will list all probes of the "mono" provider in the executable "mono" or display an error when no probes were found.

Note that using the dtrace command may require additional priviledges. On Mac OS X use `sudo`. On OpenSolaris use `pfexec` or adjust the user's priviledges (/etc/user_attr) to include `dtrace_user` and `dtrace_proc`, e.g., (as root) `usermod -K defaultpriv=basic,dtrace_user,dtrace_proc youruser`.

The mono provider
-----------------

### ves-init-begin, ves-init-end

Begin and end of runtime initialization.

With this pair of probes you can either profile the runtime initialization or use them to constrain your analysis to initialization or post-initialization.

This example script outputs the time elapsed during runtime initialization:

    mono$target:::ves-init-begin
    {
        self->start = timestamp;
    }

    mono$target:::ves-init-end
    {
        printf("%d\n", timestamp - self->start);
        self->start = 0;
    }

Run it as:

``` bash
   $dtrace -s thescript.d -q -c "mono YourApp.exe"
```

This should print the number of nanoseconds elapsed between the two probes.

### method-compile-begin, method-compile-end

Begin and end of method compilation.

The probe arguments are class name, method name and signature, and in case of method-compile-end success or failure of compilation.

### gc-begin, gc-end

Begin and end of Garbage Collection.

SGen, Mono's [Generational GC](/docs/advanced/garbage-collector/sgen/) supports many more probes, described, along with examples, on the [SGen DTrace](/docs/advanced/garbage-collector/sgen/dtrace) page.

