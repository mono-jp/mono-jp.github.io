---
title: "Accessibility: Team Meetings 2008 Jun 11"
lastmodified: '2008-06-11'
redirect_from:
  - /Accessibility%3A_Team_Meetings_2008_Jun_11/
---

Accessibility: Team Meetings 2008 Jun 11
========================================

Meeting Summary
---------------

    Attendants: bgmerrell, Calen, jpallen, MarioC, mgorse, ngao, Ray, sandy, decriptor, knocte ( & kangaroo )

    Topic—Iteration switch: 3 to 4

    (03:46:27 PM) knocte: hi
    (03:47:01 PM) sandy: MarioC: should you and I discuss what we're doing next iteration before this meeting?
    (03:47:28 PM) MarioC: sandy, do you mean the new Behavior changes?
    (03:47:38 PM) sandy: I still have a lot of work to do with my current providers, but I will probably add a new provider to the schedule anyway
    (03:47:51 PM) sandy: MarioC: no, I just mean what new providers we'll be doing
    (03:48:02 PM) knocte: guys I'm wondering: is it a good idea idea to update that wiki page everybody at the same time? I think that you can overwrite other's changes if you do it at the same time
    (03:48:19 PM) sandy: knocte: thanks, I'll change the topic now that it's closer to the meeting
    (03:48:21 PM) mode (+o knocte ) by sandy
    (03:48:30 PM) sandy has changed the topic to: Iteration 3-4 Wrap-up/Planning Meeting begins in less than 20 minutes: Accessibility:_Project_Schedule
    (03:48:56 PM) MarioC: sandy, I think we should stop adding new providers to our plans, I think that because doesn't make any sense adding "planned" to each new provider...
    (03:48:59 PM) sandy: knocte: I had that message up when it was an hour before, too
    (03:49:06 PM) MarioC: sandy, every provider is "planned", indeed
    (03:49:10 PM) knocte: ok
    (03:49:25 PM) sandy: MarioC: but we have to list what we're doing in a given iteration...
    (03:49:52 PM) knocte: I've just said that because I think this version of mediawiki doesn't check the timestamp of the last save so you can accidentally erase other's changes
    (03:50:35 PM) knocte: so it's better to agree on slots of time or something
    (03:50:40 PM) MarioC: sandy, I'm moving every default-planned provider to bottom, my idea is to finish all Edit control types, first
    (03:51:09 PM) sandy: knocte: wow, I had no idea it didn't have conflict warnings in place!
    (03:51:41 PM) knocte: sandy: I made a little test the other day and I found it out
    (03:51:47 PM) sandy: MarioC: okay, cool, then no worries...I was thinking of taking listbox or combobox depending on what knocte and calvin want
    (03:52:09 PM) sandy: knocte: that *really* sucks...can you bring that up with miguel?
    (03:52:13 PM) knocte: I would prefer combobox :)
    (03:52:23 PM) knocte: yeah I will talk to him
    (03:52:34 PM) sandy: an upgrade would be nice for other reasons, too
    (03:52:42 PM) MarioC: yes.. that's important... we should implement the providers first before the bridge is ready
    (03:52:44 PM) knocte: which other reasons?
    (03:52:47 PM) mgorse [~mgorse@130.57.22.201] entered the room.
    (03:53:07 PM) knocte: hi mgorse
    (03:53:12 PM) sandy: knocte: I don't recall exactly, but I know there have been formatting feature I've wanted to use but can't because they exist in newer versions of MW
    (03:53:21 PM) knocte: I see
    (03:53:25 PM) sandy has changed the topic to: Iteration 3-4 Wrap-up/Planning Meeting begins in less than 10 minutes: Accessibility:_Project_Schedule
    (03:53:34 PM) knocte: well anyway I think they wanted to switch to dekiwiki
    (03:53:53 PM) sandy: well, it's good to put more pressure on them to do *something*
    (03:54:00 PM) knocte: yes
    (03:54:06 PM) sandy: we can't be the only people using the wiki in this fashion where edit conflicts are likely
    (03:54:40 PM) knocte: sandy: I would doubt that, my impression is that mono devs usually work on their own pages, maybe in order to avoid this, or maybe because of their kind of work
    (03:55:02 PM) knocte: and by own pages I mean individual pages, where it's no likely many people would work
    (03:56:46 PM) MarioC: sandy, I can do ComboBox... you have already implement IScrollProvider, I can use that implementation to guide me for implementing new ComboBox's
    (03:57:03 PM) MarioC: s/ScrollProvider/SelectionProvider
    (03:57:18 PM) sandy: MarioC: cool, then I'll add listbox I think
    (03:57:37 PM) sandy: and we can also revamp all of our providers, perhaps
    (03:57:45 PM) MarioC: yes... we need to
    (03:58:16 PM) MarioC: we should add a new wiki page to describe the winforms-architecture
    (03:58:28 PM) knocte: MarioC: that sounds interesting
    (03:58:32 PM) MarioC: what do you think?
    (03:58:42 PM) mode (+o Calen ) by MarioC
    (03:58:44 PM) mode (+o calvin_ ) by MarioC
    (03:58:46 PM) mode (+o mgorse ) by MarioC
    (03:58:47 PM) knocte: above all for the people who have not dealt with it :)
    (03:58:49 PM) mode (+o ngao ) by MarioC
    (03:59:08 PM) mode (+o CIA-2 ) by MarioC
    (03:59:10 PM) knocte: well, I think the only person lacking is Ray, right?
    (03:59:28 PM) sandy: and jpallen
    (03:59:29 PM) Calen: MarioC: shall we begin our meeting?
    Calen calvin_
    (03:59:52 PM) knocte: Calen: yes, in 2 minutes, maybe they will still come
    (03:59:54 PM) MarioC: Yes, sure.
    (03:59:55 PM) Calen: MarioC: Ray said he will late some minutes
    (04:00:01 PM) knocte: oh ok
    (04:00:04 PM) sandy: I just IM'd jpallen








    (04:00:16 PM) knocte has changed the topic to: Accessibility | Iteration 4 Planning Meeting | Accessibility:_Project_Schedule#Current_Iterations
    (04:00:30 PM) knocte: Calvin asked me to run the meeting
    (04:00:41 PM) knocte: I don't know if you all received the schedule annotation
    (04:01:17 PM) knocte: I actually did a mistake and wrote "weekend" instead of "week", so I meant he was not going to be there for the week
    (04:01:28 PM) knocte: I still don't know yet if he's on FTO or in the WWDC?
    (04:02:02 PM) knocte: well, let's start, everybody ready? (if not, just tell) we'll do the usual thing
    (04:02:23 PM) knocte: each person tells summary of the week and plans for the next, and asks for help on anything if he needs to
    (04:02:44 PM) knocte: so, let's start, I'll say, mgorse?
    (04:02:50 PM) jpallen [~jpallen@137.65.132.4] entered the room.
    (04:03:08 PM) knocte: hi jpallen, we were starting the meeting, mgorse will start, if he's reading us
    (04:03:26 PM) jpallen: hello
    (04:03:27 PM) knocte: mgorse: ping ^^
    (04:03:28 PM) jpallen: sounds good
    (04:03:41 PM) mgorse: ok
    (04:03:51 PM) mgorse: I've been working on cspi still
    (04:04:13 PM) mgorse: finished the caching stuff (but haven't tested). Worked on accessible, component, table, and selection interfaces
    (04:04:29 PM) mgorse: now simple-at from the original at-spi test director ybuilds, so I've been testing with it and fixing bugs for the last two days
    (04:04:38 PM) knocte: (remember to say when you're done)
    (04:04:51 PM) mgorse: going to continue doing that until it can print out a tree of paplications that the registry registers and read events
    (04:04:59 PM) mgorse: then will start on other interfaces, such as table, if I have time this iteration
    (04:04:59 PM) mgorse: done
    (04:05:02 PM) knocte: thanks mgorse
    (04:05:14 PM) knocte: so the thing you developed the last iteration is now tested right?
    (04:05:24 PM) knocte: (you annotated it was not, yet)
    (04:05:48 PM) mgorse: not really; I'm testing it now
    (04:05:54 PM) knocte: ok
    (04:06:07 PM) knocte:  so the people who has not changed the wiki yet: let's wait until we finish the meeting
    (04:06:28 PM) knocte: as it's better not to erase anyone's changes (given the old version of mediawiki that is installed)
    (04:06:33 PM) Ray [~Ray@221.216.141.159] entered the room.
    (04:06:35 PM) knocte: now let's continue
    (04:06:41 PM) knocte: hey Ray welcome
    (04:06:43 PM) Ray: i'm sorry i'm late
    (04:06:55 PM) knocte: Ray: it's ok, only mgorse talked for now
    (04:07:03 PM) knocte: now, MarioC can you start now?
    (04:07:08 PM) MarioC: sure
    (04:07:17 PM) Ray: knocte: :)
    (04:07:26 PM) knocte: (thanks, remember to say when you're done)
    (04:07:35 PM) MarioC: I've implementing ITextProvider for TextBox, this includes the ITextRangeProvider.
    (04:08:10 PM) MarioC: I need to implement some word tokenizer classes, I'm missing Lines, Paragraphs, Documents and Pages.
    (04:08:20 PM) MarioC: s/need/needed
    (04:08:37 PM) MarioC: I need to test this provider with RichTextBox.
    (04:09:08 PM) MarioC: My plans for next iteration are: to implement IScrollProvider and ComboBox provider. And revamp old providers.
    (04:09:35 PM) MarioC: and write a wiki page to document our winforms-architecture.
    (04:09:36 PM) MarioC: done.
    (04:09:48 PM) knocte: ok, thanks MarioC can you start with ComboBox? as it's likely we'll need it shortly
    (04:09:52 PM) sandy: MarioC: cool, an architecture document...good idea
    (04:10:08 PM) MarioC: knocte, yes... sure, I can start with ComboBox
    (04:10:30 PM) knocte: I'm also wondering why we haven't needed ITextRangeProvider yet in the Atk side, as we already finished implementing the TextLabel bridge class
    (04:10:41 PM) knocte: well, let's continue, you go sandy
    (04:10:52 PM) sandy: I worked a lot on RadioButton.  Found that the container of the radio button needed to be able to implement ISelectionProvider depending on whether or not it contained any radio buttons, and since controls can be added/removed dynamically, I refactored our base provider classes to support dynamically adding/removing provider pattern support.  This iteration MarioC and I will refactor all of our providers to use this new method of attaching d
    (04:10:58 PM) sandy: Window and GroupBox made progress, too, but they are not fully tested.  I will need to write more tests for these providers, and also for RadioButton, and should be done this week.  However, there are still outstanding issues with child control/provider management that I will have to ignore until we hear back from MS, I think.
    (04:11:04 PM) sandy: esired provider pattern support.  It should clean up a lot of code (I hope).
    (04:11:05 PM) sandy: I did not work on finishing the last bits of ButtonProvider.
    (04:11:10 PM) sandy: This iteration I will also work on ListBox.
    (04:11:12 PM) sandy: done :-)
    (04:11:29 PM) knocte: heheh, now we have to finish reading :)
    (04:11:32 PM) CIA-2: sandyarm * r105580 /trunk/uia2atk/src/UIAutomationWinforms/UIAutomationWinforms/ (9 files in 3 dirs): (log message trimmed)
    (04:11:32 PM) CIA-2: * UIAutomationWinforms/Mono.UIAutomation.Winforms.mdp,
    (04:11:32 PM) CIA-2:  UIAutomationWinforms/Mono.UIAutomation.Winforms/FragmentRootControlProvider.cs,
    (04:11:32 PM) CIA-2:  UIAutomationWinforms/Mono.UIAutomation.Winforms/SimpleControlProvider.cs,
    (04:11:32 PM) CIA-2:  UIAutomationWinforms/Mono.UIAutomation.Winforms.Behaviors,
    (04:11:35 PM) CIA-2:  UIAutomationWinforms/Mono.UIAutomation.Winforms.Behaviors/RadioButtonSelectionProviderBehavior.cs,
    (04:11:38 PM) CIA-2:  UIAutomationWinforms/Mono.UIAutomation.Winforms.Behaviors/IProviderBehavior.cs:
    (04:11:51 PM) sandy: ahem
    (04:12:00 PM) knocte: ok sandy then, do you think I could work with RadioButton then for next iteration?
    (04:12:01 PM) bgmerrell: sandy:  I think it got cut off "new method of attaching d"
    (04:12:07 PM) sandy: knocte: yes
    (04:12:27 PM) knocte: ok, thanks sandy
    (04:12:31 PM) knocte: ngao is with us?
    (04:12:43 PM) ngao: yes, i'm here
    (04:12:56 PM) decriptor: sandy: have you been practicing on that typing website :)
    (04:12:59 PM) knocte: hi ngao, could you start? (remember to say when you're done)
    (04:13:09 PM) ngao: ok
    (04:13:21 PM) ngao: i finished StatusBarProviser, and added some fields in GridPatternIdentifiers
    (04:13:28 PM) ngao: i set up vista last week, so i will determine the value of IDs, and run nunit on vista.
    (04:13:35 PM) ngao: then move on to the next control.
    (04:13:44 PM) ngao: done.
    (04:14:22 PM) knocte: ok, I'm wondering if you're ok with current way of syncing with the UIA guys, or maybe you need more help from them?
    (04:15:05 PM) ngao: i've got much help form sandy and MarioC :)
    (04:15:15 PM) knocte: heh, ok, did you plan any control in particular?
    (04:15:26 PM) ngao: not yet
    (04:15:45 PM) knocte: ok, you can discuss about it with them later, to be synchronized, thanks ngao, now let's switch to QA people
    (04:15:58 PM) knocte: bgmerrell: hi! you start?
    (04:16:20 PM) bgmerrell: i worked a little on getting some demo stuff set up to demonstrate our progress
    (04:16:41 PM) bgmerrell: so i finally got to build and try things out
    (04:16:48 PM) bgmerrell: but mostly i worked on the test automation harness
    (04:17:08 PM) bgmerrell: i'm almost satisfied with it, i am just working on one or two more things
    (04:17:54 PM) knocte: finished?
    (04:17:59 PM) bgmerrell: so right now a suite of tests can be run remotely on several test machines all at once
    (04:18:09 PM) bgmerrell: but the tests are against gtk for now
    (04:18:09 PM) bgmerrell: done
    (04:18:24 PM) knocte: thanks, and you're plan for next iteration?
    (04:19:09 PM) bgmerrell: oh, right.  I want to finish up (for now) with the test harness, and start working on something similar for orca.  I also am going to help Calen get started on writing strongwind tests.
    (04:19:32 PM) bgmerrell: I need to review some standards she has come up with and document all this stuff so community people can test.
    (04:19:39 PM) bgmerrell: done again :)
    (04:19:44 PM) knocte: thanks!, would you think that it's good that the devs start using your these tests in some way?
    (04:19:57 PM) knocte: s/your/ /
    (04:20:31 PM) knocte: we can ask this also to Calen to see her opinion
    Calen calvin_
    (04:20:38 PM) knocte: Calen: ^
    (04:20:48 PM) Calen: knocte: i think maybe devs can use some of our winforms app samples :)
    (04:20:53 PM) bgmerrell: knocte: if anything you guys want to test can be tested via atspi, it can be automated and added to the test suite.
    (04:21:18 PM) sandy: Calen: are these described anywhere, or should we just poke around in svn?
    (04:21:19 PM) bgmerrell: Calen has created several winforms samples that can be tested against.
    (04:21:44 PM) knocte: yeah, I think we'll start to use it because we haven't got way to test events if not with this, thanks to both
    Calen calvin_
    (04:22:00 PM) Calen: sandy: you can take them from svn
    (04:22:03 PM) knocte: Calen: your turn, after you answer sandy :)
    (04:22:17 PM) Calen: knocte: okay
    (04:22:26 PM) Calen: I have created a wiki page for test coding standards posted in Accessibility:_Test_Coding_Standard. but it should be reviewed with Brian.
    (04:22:59 PM) Calen: in next Iteration, i will review and finish test coding standards.
    (04:23:27 PM) Calen: and update winforms application samples to abidy by the test coding standards.
    (04:24:04 PM) Calen: and start to create strongwind test scripts for winforms according to Brian's help :)
    (04:24:09 PM) Calen: done
    Calen calvin_
    (04:24:26 PM) knocte: thanks Calen
    (04:24:34 PM) knocte: interesting, there are some things in that wiki page that I see could be useful, as you guys are using Python, but maybe what about using the same policy as us the devs for file headers?
    (04:24:39 PM) knocte: what do you think sandy?
    (04:25:14 PM) ***sandy just reconnected
    (04:25:28 PM) knocte: oh, well, anyway, let's discuss this later
    (04:25:41 PM) knocte: let's switch to packaging
    (04:25:59 PM) knocte: decriptor: hi! I noticed you didn't add yourself yet to the Team wiki page, right?
    (04:26:20 PM) decriptor: no that's part of next weeks iteration :P
    (04:26:27 PM) knocte: hehe cool
    (04:26:33 PM) knocte: can you start before Ray?
    (04:26:39 PM) decriptor: sure
    (04:26:40 PM) Ray: yes
    (04:26:46 PM) Ray: I'm sorry that this week was not productive week for me.
    (04:26:56 PM) knocte: (ok, remember to say when you're done)
    (04:27:03 PM) Ray: I have tried to build mono in DEB format several times on OBS,
    (04:27:21 PM) knocte: (Ray: ok, don't worry, we can talk about, let's talk with decriptor first :) )
    (04:27:22 PM) Ray: but it failed till now, so it takes me a bit long time.
    (04:27:29 PM) Ray: sure
    (04:27:30 PM) kangaroo: Ray: talk to directhex
    (04:27:36 PM) kangaroo: He got mono debs created on obs
    (04:27:39 PM) decriptor: knocte: I'll go next :P
    (04:27:44 PM) knocte: thanks kangaroo
    (04:27:47 PM) Ray: kangaroo: thank you! :)
    (04:27:51 PM) knocte: decriptor: yeah go ahead
    (04:27:54 PM) kangaroo: np
    (04:27:59 PM) kangaroo: Ray: he usually hangs out in #mono
    (04:28:14 PM) Ray: kangaroo: ok, got it
    (04:28:31 PM) Ray: decriptor: i'm sorry, go on pls,
    (04:28:42 PM) kangaroo: (sorry for interrupting)
    (04:29:06 PM) knocte: ( kangaroo: np, thanks :) ) decriptor?
    (04:29:20 PM) decriptor: knocte: long and short, I'm learning python, building a local build server, trying to get a working laptop :/ , reading some more on rpms, spec files and learnig osc
    (04:30:22 PM) knocte: ok, cool, what do you think is you're weakest part for now? what's your plan for the next iteration? (tell when you're done)
    (04:30:31 PM) decriptor: hoping to have a working laptop today (we'll see), get that local OBS server going, put myself on the team page, and take care of some new employee stuff :)
    (04:30:35 PM) decriptor: done
    (04:30:55 PM) decriptor: weakest part right now is a none working GM of opensuse 11
    (04:30:57 PM) decriptor: :/
    (04:31:08 PM) knocte: ok, be sure to sync with Ray if you have anything to select to work on, in order to be best synced with him, or if he needs help
    (04:31:19 PM) knocte: thanks decriptor, Ray: you tell us
    (04:31:35 PM) Ray: sure
    (04:31:53 PM) jpallen: i should note that Ray is working on both packaging/build and qa
    (04:31:59 PM) jpallen: his time is split
    (04:32:07 PM) Ray: yeah
    (04:32:09 PM) knocte: oh, ok, thanks jpallen for clarifying
    (04:32:12 PM) jpallen: up until last week he has been mostly packaging
    (04:32:24 PM) knocte: then Ray: tell us both stories :)
    (04:32:29 PM) jpallen: but we had a qa meeting last week and Ray is getting more involved there now
    (04:33:06 PM) Ray: yeah, according to the last QA meeting, my jobs partially become to write test samples,
    (04:33:14 PM) bgmerrell: Calen: do you know where the wiki page is with our QA meeting?  I lost it :(
    (04:33:22 PM) Ray: so I just learnt IronPython these days,
    (04:33:29 PM) Ray: not finish a sample test script yet,
    (04:33:46 PM) Ray: and go through the test script coding standard which Calen created
    (04:34:01 PM) knocte: ok
    (04:34:04 PM) Ray: in the next iteration, I'll catch up you guys' speed, continue to learn and write samples.
    (04:34:19 PM) Ray: on the another hand, I'll talk more about our building system with decriptor.
    (04:34:41 PM) Ray: thank jpallen helps me clarifying :)
    (04:34:47 PM) knocte: ok, done Ray?
    (04:34:52 PM) Ray: and i'm over
    (04:34:58 PM) Ray: knocte: yes. :)
    (04:34:59 PM) decriptor: Ray: I forwarded you an email
    (04:35:02 PM) decriptor: check it soon
    (04:35:07 PM) Ray: decriptor: ok
    (04:35:07 PM) Calen: sorry, i think i need to mention that Ray will take over my winforms app sample creating job.
    (04:35:20 PM) knocte: ok, thanks to all, I almosft forgot, but now it's my turn :)
    (04:35:50 PM) decriptor: knocte: forgot to mention also that I'm working with the mono build manager to see if we can use the mono build environment
    (04:36:11 PM) knocte: oh thanks for pointing out decriptor
    (04:36:23 PM) knocte: well I'll start my summary and plan
    (04:36:51 PM) knocte: as Calvin said in the last meeting we were having some problems with the Atk.State class and Atk.StateSet, we found out that, again, we lacked something in the Atk bindings (thanks also to some comments by mgorse)
    (04:37:11 PM) knocte: so I implemented some bits in these bindings, with the review of mkestner, as usual
    (04:37:33 PM) knocte: I also finished some things about the control and tests of the bridge class I didn't finish in the last iteration (CheckBox)
    (04:38:05 PM) knocte: and, in the way, I also found that the new RefState implementation in atk didn't work completely, as it was having an infinite recursion in a case
    (04:38:20 PM) knocte: (which  even mkestner didn't catch)
    (04:38:39 PM) knocte: so, as he may be in vacation, I committed a harmless workaround in Atk-sharp
    (04:38:58 PM) knocte: it's working but maybe he thinks he's a bit "ugly", so we will rework it then
    (04:39:15 PM) knocte: I've also worked on the test of the ComboBox, but didn't finish it implementation yet, but
    (04:39:43 PM) knocte: as it has a few interfaces, I guess I can finish it in next iteration along with the next control, which I guess it will be RadioButton
    (04:39:43 PM) knocte: done
    (04:39:59 PM) knocte: ok, if anyone thinks we should add anything more, just tell
    (04:40:29 PM) sandy: knocte: in response to your earlier question, I think it might beOK to just having a COPYING file
    (04:40:29 PM) knocte: we'll now start changing the wiki, but in turns, because we have found that the collisions are not warned by mediawiki
    (04:40:36 PM) decriptor: sandy: will you have a chance to look at the packaging stuf for uai2atk
    (04:40:44 PM) sandy: oh, good point
    (04:40:53 PM) sandy: decriptor has brought up that packaging will be pretty hard without makefiles
    (04:41:01 PM) decriptor: not a huge deal, but if the time presents itself
    (04:41:07 PM) MarioC: what about using MD's Makefiles?
    (04:41:16 PM) sandy: MarioC: yeah, I think we'll try that first
    (04:41:18 PM) decriptor: it just needs to be enabled
    (04:41:21 PM) sandy: could be issues with dependencies though
    (04:41:27 PM) knocte: oh yeah, maybe it's a good idea to research about the makefile generation feature of MonoDevelop
    (04:41:28 PM) decriptor: that and I noticed that the dlls are in svn
    (04:41:35 PM) sandy: because our MD solution makes a lot of assumptions about our setup
    (04:41:35 PM) bgmerrell: sandy: we have this showing our WinForms samples thus far  Accessibility:_Test_Plan_WinForms_Controls
    (04:41:44 PM) knocte: yeah, I just told what MarioC pointed
    (04:41:52 PM) decriptor: knocte: it worked great for my litle project I did a while ago
    (04:42:11 PM) sandy: decriptor: I will work on it
    (04:42:14 PM) decriptor: thanks
    (04:42:32 PM) bgmerrell: sandy: and there is a (outdated) demo of the test framework in SVN with some READMEs.  I plan to get everything on a wiki this iteration
    (04:42:34 PM) decriptor: should it be cleaned before submitting too?
    (04:42:39 PM) knocte: decriptor: yeah it works well, but not with complex projects like our current ones, as they have evolved a lot and we have, glue libraries, LD_LIBRARY_PATH settings for tests...
    (04:42:47 PM) sandy: bgmerrell:  cool
    (04:43:08 PM) sandy: knocte, decriptor: also, I think maybe some of our MD projects should be separate tarballs/packages
    (04:43:09 PM) bgmerrell: knocte: you're probably interested in what i was just telling sandy, too.
    (04:43:37 PM) knocte: yeah, sounds good
    (04:43:51 PM) knocte: well first, let's say we can consider the meeting finished, thanks to all!
    (04:44:04 PM) knocte has changed the topic to: Accessibility
    (04:44:05 PM) sandy: thank you knocte for doing such a great job leading it
    (04:44:15 PM) Ray: thanks you!
    (04:44:26 PM) knocte: thanks sandy, you all have helped me much too







    (04:44:52 PM) knocte: can we all change the wiki in the same order as we have talked in the meeting?
    (04:45:09 PM) knocte: mgorse: you would go first, just tell when you're done, or tell if you want to do it later
    (04:45:16 PM) decriptor: Ray: did you get a chance to look at that email
    (04:45:39 PM) Ray: decriptor: i donwloading it, it seems a bit big :)
    (04:45:41 PM) knocte: I'll save the log of the meeting in a new wiki page
    (04:45:51 PM) decriptor: Ray: shouldn't
    (04:46:10 PM) decriptor: its just tezt
    (04:46:12 PM) decriptor: text
    (04:46:26 PM) Ray: decriptor: oh, or maybe someone send a attached email before you. :)
    (04:46:48 PM) sandy: knocte: I may not get to the wiki for a little while
    (04:47:07 PM) ***sandy tried to undock his laptop the "right" way and now it's very angry
    (04:47:12 PM) knocte: sandy: ok thanks don't worry, we'll jump to the next
    (04:47:38 PM) knocte: mgorse seems to be unavailable right now, so, MarioC: you go on the wiki if you can
    (04:47:55 PM) MarioC: he's back
    (04:48:05 PM) knocte: ok, let's wait for him
    (04:48:19 PM) Ray: decriptor: it's about 8M attached file, so it's a little bit slow. :(
    (04:48:31 PM) decriptor: eh
    (04:48:35 PM) knocte: well, now I'm thinking that it may be better to go in the inverse order, as the chinese people would want to go to bed? :)
    (04:48:53 PM) knocte: or maybe they will do it tomorrow..
    (04:49:31 PM) mgorse: ok, sorry; was afk. I can go now or later; doesn't matter
    (04:49:33 PM) Ray: knocte: evening meeting is ok for me. :)
    (04:50:08 PM) mgorse: okay, I'll just do it now--shouldn't take long
    (04:50:09 PM) ngao: knocte: it's ok
    (04:50:28 PM) knocte: ok, let's china people jump just after mgorse
    (04:50:34 PM) bgmerrell: afk for a bit
    (04:50:41 PM) knocte: mgorse: thanks, tell us when you're done
    (04:50:54 PM) Ray: decriptor: oh yeah, i have received this mail
    (04:51:28 PM) sandy: guys, has your laptop ever beeped at you when you tried to close it?
    (04:51:42 PM) mgorse: sandy: yeah, it does now that I've upgraded to 11
    (04:51:50 PM) sandy: mgorse: do you know why/when?
    (04:52:10 PM) sandy: this is the first time I've undocked my laptop since upgrading, I think
    (04:52:48 PM) sandy: I used the undock button before the eject button (on the dock itself) and the laptop screen wouldn't show me anything
    (04:52:54 PM) sandy: then putting it back in the dock I couldn't get to X
    (04:52:56 PM) sandy: it was really weird
    (04:53:17 PM) sandy: and when closing the laptop it made an alarming tone
    (04:53:56 PM) mgorse: okay, I'm done
    (04:54:07 PM) knocte: ok, ngao, can you edit the wiki page now?

...

