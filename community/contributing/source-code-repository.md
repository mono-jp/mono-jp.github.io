---
title: Source Code Repository
redirect_from:
  - /SourceCodeRepository/
  - /AnonSVN/
  - /SVN/
---

The Mono source code is hosted on [GitHub](https://github.com) using the [Git](http://git-scm.com/) source code control system for all of its source code. Although only active contributors get write access to the modules on Git, third party developers and easily fork the code on GitHub or download full copies of the repositories to their own systems.

Here we describe how one obtains commit access to the Mono Git repository and the responsibilities that come with that access privilege.

Browsing the Sources
--------------------

If all you need is to browse the sources, you can go to [Mono Organization page on GitHub](https://github.com/mono).

Building Mono from source
-------------------------

Once you've obtained the source code for different modules of the Mono project, you'll want to [build Mono from source](/docs/compiling-mono/)

Contributing Patches
====================

Now that Mono is hosted on GitHub, contributing patches has never been easier. If you aren't yet familiar with GitHub, you may wish to read GitHub's guide on [getting started](https://help.github.com/articles/set-up-git/).

Once you've gotten a GitHub account and gotten set up, you should read GitHub's guide to [forking a repository](https://help.github.com/articles/fork-a-repo/). Once you feel that your patch is finished and you've tested that everything still builds and works as expected, you can then issue a [pull request](https://help.github.com/articles/using-pull-requests/) which alerts the active maintainers that they should examine and review your patch, merging it into the mainline source repository.

Policies
========

It is important that everyone follow these policies:

### Coding Guidelines

We have our own [coding guidelines](/community/contributing/coding-guidelines/).

### Code License

If you are about to commit code to a module, the code that is being committed should be released under the MIT license.

If in doubt, check with the maintainers of the module, or send mail to mono-devel-list@ximian.com.

### Changing Code

Even if you have write access to the official Mono Project GitHub repositories, that doesn't mean you can change code at will in any directory or module. Directories and Namespaces have a sort of unofficial ownership. If you are not the owner of a piece of code and you want to make changes/fixes to it, there are two cases.

-   The change is a typo fix or a one-liner build or trivial fix. In this case almost anyone can commit (always remembering to add the proper changelog entry to explain the change). We say "almost anyone", because changes to certain directories almost always should be reviewed first. Such as changes to core stuff: corlib/System, System.Collections, mini/, metadata/, System.IO.

-   The change is larger. In this case the patch **must** be sent to mono-devel-list for review by the owner of the code and by the other hackers. Always submit such patches to the list or bugzilla, although you may put the owner of the code in the CC header. Hackers come and go. Mailing a patch to only a personal address is a good way to get the patch forgotten and missed. Plus, getting the patches reviewed as well as reviewing them, is a good thing, so try to get used to it.

Note: If the patch is an addition of code and doesn't change any of the existing code, the rules are slightly relaxed: there is more freedom in committing such changes, if they don't interfere with the existing codebase.

### Owning Code

Now, how do you get to be the owner of a chunk of code? The answer is simple. You wrote the code, so you're the unofficial owner. There is also another way. After sending a few patches for the code, the owner (or the core developers of mono, if the owner somehow disappeared) trusts you and tells you you're free to commit without getting his review first.

You can most likely find ownership by reading ChangeLogs or by using `git blame`. The entries are with emails, so feel free to ask them. If you are still unsure, post your patch to the mailing list (mono-devel-list).

If you are the owner of a piece of code, feel free to commit code, and delegate the work to others.

But, if you're not the owner of the code, committing a rewrite without getting a review first is frowned upon (especially when the rewrite claimed to fix bugs, but not a single regression test has been added to the suite).

### Pull-Request Rules

There are a few rules to follow before making a pull request on GitHub:

-   Sign the [.NET Foundation CLA](https://cla2.dotnetfoundation.org)

-   Always make sure to add meaningful commit logs

-   If you fix a bug, add a regression test for it in the [test suite](/community/contributing/test-suite/)

-   Don't commit unrelated changes together with a fix: do fine-grained commits

-   Always check what you're committing: make sure you're only committing what you need and make sure you don't change line endings and whitespace. Do a `git diff` of the files you're going to commit and check the changes.

-   Don't do reformatting commits, unless you're the original author of the code

-   When fixing bugs, don't follow the documentation blindly, it may well be wrong. Test the behavior on the MS runtime or ask on the list for discussion if unsure. Don't be afraid of having your changes reviewed.

-   Never remove copyright notices from the code

-   Never remove licensing info from code

-   Never commit code you didn't write yourself or code that doesn't have a suitable license

-   For documentation fixes, never copy paste documentation from Visual Studio class view or MSDN.

-   Never use a decompiler or disassembler to look at proprietary code.

-   Follow the [coding guidelines](/community/contributing/coding-guidelines/)

-   Keep an eye on performance considerations, especially for code in core classes, ask on the list for guidance

-   Do a regression test run and a bootstrapping build if making changes to core functionality before committing. Do not commit code that would break the compile, because that wastes everybody's time. Two things are important in this step: trying to build your sources and making sure that you add all the new files before you do a commit.

Also, remember to pat yourself on the back after the commit, smile and think we're a step closer to a better free software world.

Getting Help With Git
=====================

GitHub maintains some great resources for developers here:

[https://help.github.com/](https://help.github.com/)

Keeping track of code changes
=============================

### Via Email

We provide an e-mail based mechanisms to keep track of changes to the code base:

-   [mono-patches](http://lists.ximian.com/mailman/listinfo/mono-patches): This mailing list receives in patch form all the changes that are being made to git. To subscribe, send an email message to mono-patches-request@ximian.com and in the body of the message put \`subscribe' or click on the link.

This will send you an email message every time a change is made to the git repository, together with the information that the author of the changes submitted.
