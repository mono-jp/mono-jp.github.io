---
title: "Accessibility: Team Meetings 2008 Sep 10"
lastmodified: '2008-09-10'
redirect_from:
  - /Accessibility%3A_Team_Meetings_2008_Sep_10/
---

Accessibility: Team Meetings 2008 Sep 10
========================================

    (04:00:36 PM) knocte has changed the topic to: Iteration switch meeting
    (04:01:13 PM) knocte: ok, now that poor sandy is not with us (I hope he's ok, although maybe he needs surgery :( ), I'll let brad start
    (04:01:27 PM) brad: hey folks
    (04:01:47 PM) knocte: so go ahead
    (04:01:48 PM) brad: so this week, I'd like everyone to pick something that they've worked on before, and see it through to 100% complete
    (04:02:03 PM) brad: we need to start checking things off our list so we can make progress on the larger widgets
    (04:02:24 PM) brad: this week will be business as usual, but I'd like us to start doing the daily updates starting next wednesday
    (04:02:50 PM) brad: hopefully we'll have a better idea of how many hours remain, and can have better iteration assignments that way by then
    (04:03:10 PM) brad: so my task for this week is to finish up the Functional Spec, and to start putting estimates beside each task
    (04:03:26 PM) brad: so we can better schedule iterations
    (04:03:34 PM) brad: okay, that's all I have
    (04:03:45 PM) knocte: thanks brad; we also should focus on bugs with priority P1, right? as they are important for the smoke tests
    (04:03:55 PM) brad: yes, that should go without saying
    (04:04:05 PM) brad: bugs should always have higher priority than new work
    (04:04:45 PM) brad: btw, I just got an update from Sandy's wife... he's doing better and responding to new medication, and probably won't need surgery
    (04:05:02 PM) knocte: that sounds great
    (04:05:07 PM) bgmerrell: good news
    (04:05:10 PM) knocte: ﻿perfect, then regarding this target for the iteration, let's change what you had in mind for the "plan" part of your statuses reports
    (04:05:49 PM) knocte: so, can we start with mario then? everybody here? I guess yes
    (04:05:59 PM) mario: Hello!
    (04:06:17 PM) knocte: go ahead ;)
    (04:06:29 PM) mario: in this iteration I finished all tooltip-based providers. I need to open bugs to commit the patches in mcs
    (04:06:46 PM) mario: I fixed some bugs in our side
    (04:07:07 PM) mario: I'll spend my next iteration in bugzilla, fixing, opening and closing bugs.
    (04:07:26 PM) mario: btw
    (04:07:39 PM) mario: there's a new page
    (04:07:39 PM) mario: Accessibility:_Implementation
    (04:07:45 PM) mario: that shows the missing events in the providers
    (04:08:12 PM) mario: we (and ngao and sandy) should implement missing events
    (04:08:23 PM) mario: done
    (04:08:53 PM) knocte: so in this iteration, you're also going to implement missing events on providers done in past iteration?
    (04:09:09 PM) jpallen [~jpallen@137.65.132.22] entered the room.
    (04:09:22 PM) mario: knocte: I'll try, however my priority is to fix the bugs
    (04:09:35 PM) ray: jpallen, hello :)
    (04:09:41 PM) knocte: sure, I hope the bugs are not to complex
    (04:09:51 PM) knocte: hello jared, we were starting the meeting
    (04:10:08 PM) jpallen: hello everyone
    (04:10:10 PM) jpallen: sorry i'm late
    (04:10:15 PM) mode (+o jpallen ) by brad
    (04:10:26 PM) mario: Yes, I don't think so. I'm wrestling right now with accerciser and the frozen console. that's the only problem right now
    (04:10:50 PM) mario: done done!
    (04:10:50 PM) knocte: ok
    (04:11:02 PM) knocte: nice, then let's go with neville
    (04:11:06 PM) knocte: ngao: you here?
    (04:11:15 PM) ngao: yes
    (04:11:32 PM) ngao: last iteration, i was working on status bar navigation, encountered a problem that status bar couldn't find  its children. i am blocked with this issue now, i would like to reopen bug#419079, but i haven't found how to fix it.
    (04:12:18 PM) ngao: i will fix it next iteration as soon as possible.
    (04:12:18 PM) ngao: done
    (04:12:33 PM) knocte: fine, thanks
    (04:12:51 PM) knocte: mgorse: your turn please
    (04:13:15 PM) mgorse: okay.  I've mostly been working on 418524 still.  I finally have a patch that works for me.
    (04:13:30 PM) mgorse: Ie, passes keys / lets Orca see them
    (04:14:49 PM) mgorse: I also committed some fixes to the bridge tester and tried to look at 542873 (at-spi not seeing tooltips, from gail at least) but didn't make much progress there
    (04:15:07 PM) mgorse: Next iteration I'm going to get my code committed for 418524 and look at what's still failing in the bridge
    (04:15:23 PM) mgorse: and I'd like to try to get to the bottom of 542873 but don't really know what's going on right now
    (04:15:24 PM) mgorse: done
    (04:15:35 PM) knocte: ok, do you have any uncompleted widget in the bridge?
    (04:16:04 PM) knocte: good job on the orca end, I guess that's cool for enabling a new bunch of QA  tests
    (04:16:24 PM) knocte: I'll take a look on the patches
    (04:16:24 PM) mgorse: knocte: I think that scrollbar still needs some work.  At least one of the tests is failing for it.
    (04:16:52 PM) knocte: ok, thanks mgorse, then concentrate on it if you finish with P1 bugs
    (04:18:13 PM) knocte: then switching to me, I spent this iteration mainly with the functional spec and plan to help on that for next iteration as well, specially on the provider side, also fixed some things in some bits in the bridge, and I plan to finish the textbox widget and P1 bugs, which
    (04:18:48 PM) knocte: which sadly are often re-directed to the providers, so mario will get angry (just found out that a call to an InvokeProvider is blocking) :)
    (04:19:13 PM) knocte: ok, so let's go with QA now, calen: you here?
    (04:19:23 PM) calen: i am here
    (04:19:49 PM) knocte: fine, go ahead
    (04:19:53 PM) calen: in this iteration i have commited new strongwind test code for progressbar and numericupdown controls. modified some old test code   for indentation issue, deleted some unuseful description, add sleep time for setting value
    (04:20:06 PM) calen: re-runed all strongwind tests those i have finished, and file a list to descript which bugs blocking us from using strongwind automation test. and file a new bug for checkbox control. virified some bugs
    (04:20:14 PM) calen: spent a little time talking to Ray about Orca test and smoke test.
    (04:20:23 PM) calen: next iteration, i will keep on write strongwind test, virify bugs, update Test_Plan_WinForms_Controls wiki page.
    (04:20:25 PM) calen: done
    (04:20:36 PM) knocte: thanks calen
    (04:20:40 PM) knocte: ﻿( jpallen: in case you want to review what you missed: http://monoport.com/37258 )
    (04:20:56 PM) knocte: let's go with Brian now
    (04:21:09 PM) knocte: bgmerrell: here?
    (04:21:14 PM) bgmerrell: This iteration I wrote a couple of Gtk Orca example tests.  They are in uia2atk/test/keystrokes.
    (04:21:52 PM) bgmerrell: I struggled with some oddness that occurs when testing with Orca's flat review keyboard commands, but I got those issued cleared up on the Orca mailing list.
    (04:22:03 PM) bgmerrell: I also wrote the documentation on how we will use Orca's existing test harness to perform our tests.
    (04:22:15 PM) bgmerrell: Accessibility:_Testing_Howto#Orca
    (04:23:16 PM) bgmerrell: this iteration i will be focused on getting the automated smoke tests put together
    (04:23:42 PM) bgmerrell: I have a lot of code that i need to review, too, but I am guessing I won't get to that this iteration ... maybe i will
    (04:23:45 PM) bgmerrell: done
    (04:24:07 PM) knocte: thanks brian
    (04:24:31 PM) knocte: let's go with Ray: QA first please :)
    (04:24:38 PM) ray: ok, it's my turn
    (04:24:46 PM) ray: so in this week, i have ThreadExceptionDialog control done.
    (04:25:05 PM) ray: but there are 4 datagrid* controls and WebBrowser, HelpProvider which has not been implemented,
    (04:25:24 PM) ray: kind bgmerrell helps me out to take care of datagrid*, i thought about postpone the implementation of the rest two controls due to the Mono libraries have some issues with these.
    (04:25:35 PM) ray: and i have done RPMs smoke test for several times.
    (04:25:59 PM) ray: for the build part,  i have the latest UiaAtkBridge and olive built on openSUSE 11.0 platform, but UIAutomation seems has some problems.
    (04:26:17 PM) ray: and i was also thinking about establish a local build server in Beijing for many of us. i can use my desktop as the server machine , what do you think?
    (04:26:22 PM) ray: thanks, done
    (04:26:54 PM) knocte: thanks ray; I guess it sounds good if it helps you in any way, unless it's a lot of work
    (04:27:04 PM) knocte: the nunit issue was already solved right?
    (04:27:22 PM) sshaw: knocte: sandy took care of that
    (04:27:26 PM) ray: knocte, yes, i configure it with --disable-tests option
    (04:27:40 PM) knocte: cool
    (04:28:15 PM) knocte: I know other places where they never run the tests by default, and they have a make target for that
    (04:28:21 PM) knocte: it's another option
    (04:28:34 PM) knocte: well, let's talk with sshaw now
    (04:29:19 PM) ray: knocte, make sense
    (04:29:47 PM) sshaw: working on build stuff.  Just keeping up with the changes in trunk and resulting changes that need to happen in the spec file.  Also worked a little with brian on starting to get the smoke tests automatically kicked off when I push rpms
    (04:30:25 PM) sshaw: started looking at other CI (continuous integration) systems.  Fireball (from medsphere) and cruise control
    (04:30:42 PM) sshaw: seen some really impressive things there.
    (04:31:39 PM) sshaw: this next iteration I'll continue working on this stuff
    (04:31:49 PM) sshaw: and fixing rpms as problems arise
    (04:31:50 PM) sshaw: done
    (04:31:55 PM) knocte: sshaw: sounds good, BTW, is there a way to know the SVN revision of the source code that corresponds to an rpm?
    (04:32:09 PM) sshaw: its in the rpm name :)
    (04:32:37 PM) sshaw: so mono-core-112581-0.novell.i586.rpm was built from rev 112581
    (04:32:51 PM) knocte: oh cool, then this is one thing I wanted to mention to QA, in bugs, please attach rev number rather than the date of an rpm, ok? thanks :)
    (04:33:37 PM) calen: knocte: okay
    (04:33:37 PM) sshaw: there is a list of dates on this site that has the rpms.  You can go back and reference the rev number of the rpms from that dayhttp://build1.sled.lab.novell.com/uia/
    (04:34:02 PM) knocte: sshaw: nice to know as well, thanks sshaw
    (04:34:07 PM) knocte: ﻿so I guess we're done, did I miss anyone? jpallen: do you want to arise anything?
    (04:34:39 PM) jpallen: sure
    (04:34:50 PM) jpallen: i assume you have all seen my e-mail this week
    (04:35:07 PM) jpallen: the goal is to get automated smoke tests running by the end of the week
    (04:35:30 PM) jpallen: for those of you that have P1 bugs, thank you for looking into them
    (04:36:20 PM) jpallen: once those bugs are fixed, qa can get the first of our automation running
    (04:36:32 PM) jpallen: and we will remain automated from here on out
    (04:36:49 PM) jpallen: mono 2.2 is freezing at the end of the month
    (04:37:11 PM) jpallen: they will be releasing in nov/dec
    (04:37:37 PM) jpallen: i want us to have a release as well
    (04:38:09 PM) brad: sounds good
    (04:38:26 PM) jpallen: i want to be able to communicate outside that we have certain widgets that are feature complete and at least accessible via something like accersiser (sp?)
    (04:38:42 PM) jpallen: this means we need to take care as we submit patches to mono
    (04:38:47 PM) jpallen: sounds like mario has a few more?
    (04:39:00 PM) mario: yes. only 1
    (04:39:02 PM) jpallen: please be aware of their feature freeze schedule (end of this month, no hard date yet)
    (04:39:48 PM) jpallen: if our patches are not submitted in time for mono freeze, then they will not get included in their qa cycle which means they will not make it in to the next release (in this case, v 2.2)
    (04:40:10 PM) jpallen: so, as knocte and brad pointed out
    (04:40:19 PM) jpallen: we need to see these widgets to completion
    (04:40:51 PM) jpallen: knocte and brad will be compiling a list of widgets that will be ready for the mono 2.2 release
    (04:41:17 PM) jpallen: sound good?
    (04:41:19 PM) jpallen: any questions?
    (04:41:33 PM) knocte: I would add that our patches normally just add some events and harmless bits that I guess it's difficult that could cause any regression, right? so it would be great if we are allowed to backport to the branch if we *really* need it
    (04:42:09 PM) jpallen: the problem is that these are patches to mono
    (04:42:10 PM) knocte: we'd have to talk about it with the winforms team I guess..
    (04:42:16 PM) knocte: yes
    (04:42:17 PM) jpallen: so it affects their qa
    (04:42:24 PM) knocte: I see
    (04:42:35 PM) jpallen: if we backport, then we would be responsible for regression testing of all of winforms
    (04:42:48 PM) jpallen: that would not be good ;-)
    (04:42:52 PM) knocte: good point
    (04:44:08 PM) jpallen: also, once the functional spec is completed, we will see some more stringent assignment of responsibiliteis
    (04:44:11 PM) jpallen: in other words, developers will be assigned specific widgets and will be responsible for completing them on schedule
    (04:44:52 PM) jpallen: brian, please keep us posted on our progress toward our goal for the week
    (04:45:07 PM) bgmerrell: roger
    (04:45:16 PM) jpallen: thanks everyone, for your hard work
    (04:45:20 PM) jpallen: keep it up! :-)
    (04:45:22 PM) jpallen: done
    (04:45:27 PM) knocte: thanks jpallen!
    (04:46:01 PM) knocte has changed the topic to: Accessibility: Accessibility
    (04:46:18 PM) brad: thanks guys!  as usual, please send any feedback to the ideas i've proposed

