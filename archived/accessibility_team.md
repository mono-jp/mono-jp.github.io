---
title: "Accessibility: Team"
lastmodified: '2010-07-15'
redirect_from:
  - /Accessibility%3A_Team/
---

Accessibility: Team
===================

A page to assist in getting new team members up to speed and to lay out procedures of how the team works.

<table>
<col width="100%" />
<tbody>
<tr class="odd">
<td align="left"><h2>Table of contents</h2>
<ul>
<li><a href="#vpn">1 VPN</a></li>
<li><a href="#team-members">2 Team Members</a>
<ul>
<li><a href="#former-team-members">2.1 Former Team Members</a></li>
</ul></li>
<li><a href="#getting-started">3 Getting Started</a></li>
<li><a href="#planet">4 Planet</a></li>
<li><a href="#team-meetings">5 Team Meetings</a></li>
</ul></td>
</tr>
</tbody>
</table>

### VPN

For some things it's interesting to be connected to Novell VPN (for instance, to access [some build pages](http://build1.sled.lab.novell.com/uia/)). So go ahead and install the package **NetworkManager-novellvpn-gnome** (which will pull others like **NetworkManager-novellvpn**, **novell-nortelplugins** and **novell-ipsec-tools**).

After that, you have to configure the VPN connection. Left-click on NM notification icon (systray) -\> VPN Connections -\> Configure VPN... -\> Add -\> Forward. Then you should see a combo box which contains the item "NovellVPN Client". If you don't see it, you have to restart the OS or NetworkManager for the new module that you just installed, to be loaded.

Then, after you select NovellVPN Client on the combo, click Forward again. You need to fill some fields (leave the ones not mentioned as is):

-   **Connection Name**: NovellVPN
-   **Gateway**: vpn.emea.novell.com *(or the corresponding to your area)*
-   **User Name**: *\<your innerweb username\>*
-   **Group Name**: novell

After that, to connect: Left-click on NM notification icon (systray) -\> VPN Connections -\> NovellVPN. You will then be requested 2 passwords: the normal one is your innerweb's password, and the second is a global novell password, request it in the channel ;)

### Team Members

You can see a list of hackergotchis here along with their corresponding roles on the team, and links to their blogs:

[![Calen.png](/archived/images/5/59/Calen.png)](/archived/images/5/59/Calen.png)

**Calen Chen**
*a11y QA Hacker*
*[Calen in Novell](http://calen-innovell.blogspot.com)*

[![Hackergotchi-mario.png](/archived/images/b/b5/Hackergotchi-mario.png)](/archived/images/b/b5/Hackergotchi-mario.png)

**Mario Carrion**
*a11y Technical Lead & Hacker*
*[it's gotta be smooth](http://blog.carrion.ws/)*

[![None.png](/archived/images/e/e3/None.png)](/archived/images/e/e3/None.png)

**Mike Gorse**
*a11y Hacker*
*[wanderings of an aimless vortex](http://lightvortex.livejournal.com)*

[![Ngao.png](/archived/images/e/e9/Ngao.png)](/archived/images/e/e9/Ngao.png)

**Neville Gao**
*a11y Hacker*
*[Neville's Blog](http://figod.blogspot.com/)*

[![Ray.png](/archived/images/3/34/Ray.png)](/archived/images/3/34/Ray.png)

**Ray Wang**
*a11y Build Hacker*
*[Ray Wang's Blog](http://gnuray.blogspot.com)*

[![None.png](/archived/images/e/e3/None.png)](/archived/images/e/e3/None.png)

**Stephen Shaw**
*a11y Build Hacker*
*[Decriptor's Blog](http://www.decriptor.com)*

[![None.png](/archived/images/e/e3/None.png)](/archived/images/e/e3/None.png)

**FengXia Mu**
*a11y QA Hacker*
*[FengXia Mu](http://fengxiamu.spaces.live.com/)*

[![Matt.png](/archived/images/0/0a/Matt.png)](/archived/images/0/0a/Matt.png)

**Matt Guo**
*a11y Hacker*
*[Matt Guo](http://blog.mattguo.com)*

#### Former Team Members

[![Knocte.png](/archived/images/5/54/Knocte.png)](/archived/images/5/54/Knocte.png)

**Andrés G. Aragoneses**
*a11y Prj Manager and Hacker*
*[knocte::MonoTema](http://knocte.blogspot.com)*

[![None.png](/archived/images/e/e3/None.png)](/archived/images/e/e3/None.png)

**Brad Taylor**
*a11y Team Lead*
*[the chronicles of me](http://brad.getcoded.net)*

[![Bgmerrell0.png](/archived/images/1/17/Bgmerrell0.png)](/archived/images/1/17/Bgmerrell0.png)

**Brian Merrell**
*a11y QA Hacker*
*[Brian's lovable online gazette](http://bgmerrell.blogspot.com)*

[![Sandy.png](/archived/images/4/4e/Sandy.png)](/archived/images/4/4e/Sandy.png)

**Sandy Armstrong**
*a11y Hacker*
*[5:55 AM](http://automorphic.blogspot.com)*

### Getting Started

Things that each member needs to have set up

-   Your primary booting OS should be [openSUSE](http://www.opensuse.org) 11.1 (or later)
-   Send your blog to [Andrés](mailto:aaragoneses@novell.com).
    -   Create one if you don't have one, you'll need it.
-   Send [Andrés](mailto:aaragoneses@novell.com) your [hackergotchi](http://en.wikipedia.org/wiki/Hackergotchi) for this page
-   Join accessibility mailing lists
    -   [mono-a11y](http://forge.novell.com/mailman/listinfo/mono-a11y) - this is the team mailing list
    -   Accessibility lists of interest
-   Live on IRC
    -   \#mono-a11y on irc.gimp.org. [Direct link](irc://irc.gnome.org/mono-a11y)
-   Review everything on the [Accessibility](/Accessibility) wiki page

### Planet

There's really not an official planet for accessibility right now, because:

-   [David Bolter's one](http://aplanet.atrc.utoronto.ca/) didn't have a proper top-level or 2nd level domain.
-   Recently new created [www.planet-a11y.net](http://www.planet-a11y.net/) hasn't collected all the bloggers from previous planet yet, and the admin roles have to be worked out.

In the meantime, we'll request to the [LinuxFoundation](http://www.linuxfoundation.org) the creation of [planet.a11y.org](http://planet.a11y.org) as another useful redirection for the latter.

### Team Meetings

-   [2009, Feb 09](/Accessibility:_Team_Meetings_2009_Feb_09) IRC - 1.0 Feature Freeze Planning
-   2009, Jan 07 IRC - Sprint 5 Planning
-   [2008, Dec 10](/Accessibility:_Team_Meetings_2008_Dec_10) IRC - Sprint 4 Planning
-   [2008, Nov 26](/Accessibility:_Team_Meetings_2008_Nov_26) IRC - Sprint 3 Planning
-   [2008, Nov 12](/Accessibility:_Team_Meetings_2008_Nov_12) IRC - Sprint 2 Planning
-   [2008, Oct 29](/Accessibility:_Team_Meetings_2008_Oct_29) IRC - Sprint 1 Planning
-   [2008, Oct 15](/Accessibility:_Team_Meetings_2008_Oct_15) IRC - Iteration 19 Planning
-   [2008, Oct 01](/Accessibility:_Team_Meetings_2008_Oct_01) IRC - 1st 2week iteration Planning
-   [2008, Sep 17](/Accessibility:_Team_Meetings_2008_Sep_17) IRC - Iteration 17 Planning
-   [2008, Sep 10](/Accessibility:_Team_Meetings_2008_Sep_10) IRC - Iteration 16 Planning
-   [2008, Sep 03](/Accessibility:_Team_Meetings_2008_Sep_03) IRC - Iteration 15 Planning
-   [2008, Aug 20](/Accessibility:_Team_Meetings_2008_Aug_20) IRC - Iteration 14 Planning
-   [2008, Aug 13](/Accessibility:_Team_Meetings_2008_Aug_13) IRC - Iteration 13 Planning
-   [2008, Aug 06](/Accessibility:_Team_Meetings_2008_Aug_06) IRC - Iteration 12 Planning
-   [2008, Jul 30](/Accessibility:_Team_Meetings_2008_Jul_30) IRC - Iteration 11 Planning
-   [2008, Jul 23](/Accessibility:_Team_Meetings_2008_Jul_23) IRC - Iteration 10 Planning
-   [2008, Jul 16](/Accessibility:_Team_Meetings_2008_Jul_16) IRC - Iteration 9 Planning
-   [2008, Jul 09](/Accessibility:_Team_Meetings_2008_Jul_09) IRC - Iteration 8 Planning
-   [2008, Jul 02](/Accessibility:_Team_Meetings_2008_Jul_02) IRC - Iteration 7 Planning
-   [2008, Jun 25](/Accessibility:_Team_Meetings_2008_Jun_25) IRC - Iteration 6 Planning
-   [2008, Jun 18](/Accessibility:_Team_Meetings_2008_Jun_18) IRC - Iteration 5 Planning
-   [2008, Jun 11](/Accessibility:_Team_Meetings_2008_Jun_11) IRC - Iteration 4 Planning
-   [2008, Jun 04](/Accessibility:_Team_Meetings_2008_Jun_04) IRC - Iteration 3 Planning
-   [2008, May 28](/Accessibility:_Team_Meetings_2008_May_28) IRC - Iteration 2 Planning
-   [2008, May 15](/Accessibility:_Team_Meetings_2008_May_15) IRC - Team Meeting
-   [2008, Aug 13](/Accessibility:_QA_Meetings_2008_Aug_13) IRC - QA Meeting #2
-   [2008, Jun 5](/Accessibility:_QA_Meetings_2008_Jun_5) IRC - QA Meeting #1

(Generated using [Irc2Wiki](/Irc2Wiki))

