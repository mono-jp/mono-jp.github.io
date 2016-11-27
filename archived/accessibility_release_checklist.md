---
title: "Accessibility: Release Checklist"
lastmodified: '2009-03-13'
redirect_from:
  - /Accessibility%3A_Release_Checklist/
---

Accessibility: Release Checklist
================================

Release Checklist
=================

1.  Come up with [release codename](http://en.wikipedia.org/wiki/List_of_Futurama_characters)
2.  Edit NEWS
3.  Update ChangeLog and double-check version in configure.ac
4.  Distcheck
    1.  `make distcheck`

5.  **COMMIT CHANGES**
6.  Run automated QA scripts, get QA sign-off. Test on openSUSE 11.0/11.1 for 32 and 64 bit.
7.  Tag release
    1.  `svn cp svn+ssh://mono-cvs.ximian.com/source/branches/uia2atk/1.0 svn+ssh://mono-cvs.ximian.com/source/tags/uia2atk/$VERSION`
    2.  Commit Message: "Tag for \$VERSION release"
    3.  Double check it worked: [http://anonsvn.mono-project.com/viewvc/tags/](http://anonsvn.mono-project.com/viewvc/tags/)

8.  Build tarballs and RPMs for openSUSE 11.0/11.1 for 32 and 64 bit.
9.  Increment version in configure.ac on trunk/branch (wherever the tag was made from)
10. Upload the release
    1.  TODO:

11. Edit [releases](/Accessibility:_Releases?action=edit) wiki page
12. Add Release Notes wiki page (e.g.: Accessibility:_Release_Notes_0.9.1)
13. Update [homepage](/Accessibility?action=edit)
    1.  Use data from the [NEWS page](http://anonsvn.mono-project.com/viewvc/trunk/uia2atk/NEWS) to populate the page

14. Email [mono-a11y list](mailto:mono-a11y@forge.novell.com), [mono-announce list](mailto:mono-announce-list@lists.ximian.com) and [gnome-announce list](mailto:gnome-announce-list@lists.gnome.org)
15. Change #mono-a11y's topic


