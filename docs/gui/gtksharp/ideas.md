---
title: GtkSharpIdeas
redirect_from:
  - /GtkSharpIdeas/
---

Here we are tracking ideas that we would like to integrate into the [Gtk#](/docs/gui/gtksharp/) API.

Data Binding
============

We want to support Data Binding, but we need someone with experience on Data Binding to spec out the requirements and expected behavior of forms that use it.

OpenGL integration
==================

The [Tao Framework](/Tao) provides complete bindings to OpenGL, the issue is how to create window regions in Gtk# that can host OpenGL areas.

There is a Gtk# widget that integrates OpenGL [here](http://www.olympum.com/~bruno/gtkgl-sharp.html)

Rendering
=========

Cairo integration
-----------------

Integration from Cairo should be revisited as Cairo evolves. There are two problems in adopting Cairo today as part of the core rendering engine of Gtk#:

-   Mono.Cairo depends on Cairo which is still a moving target and the API frequently changes.
-   Cairo must support Win32 if we want to make this part of the of the cross-platform functionality.

The Gtk group has adopted Cairo as their rendering engine for future versions of Gtk, so it might make sense to just wait for them.

TreeView
========

The TreeView is considered fairly complex, integration with DataSet/DataTable would help here, maybe provide a default widget that would just do this integration?

Tutorials
=========

People are interested in more in-depth tutorials, the question is what subjects.

A few subjects suggested:

-   How to set the values on a ComboBox to a ListStore?
-   App Framework:
    -   Menus
    -   Accelerators
    -   Toolbars
    -   Session management? (Better not ;-)

-   [Developing Responsive Applications](/docs/gui/gtksharp/responsive-applications/) (Work-in-Progress).

-   Deployment: confusion about which installer to use (there are three available).

-   More example programs, or make the current ones more visible.

Documentation
=============

Gtk# documentation not complete. Samples wanted.

Widgets
=======

Interest in having widgets to do:

-   Grids (spreadsheet-like, for data entry)
-   NPlot/Gtk working on Windows (currently hardcodes the gdk_x11 stuff, copy the stuff over from GtkDotNet.dll)
-   DataGrids (same, but bound to System.Data in some form)
-   GnomeCanvas on the Windows port.
-   Simple API for trees: instead of a model/view split, have the model/view be self contained:

<!-- -->

     p = new Node ("Hello");
     p.Append (new Node ("child1"));
     p.Append (new Node ("child2"));

Other Libraries
===============

-   Support Audio in some form (SDL?)

Platforms
=========

Discussion on [Improving Gtk+ on Windows](/archived/improvinggtkwin32)

