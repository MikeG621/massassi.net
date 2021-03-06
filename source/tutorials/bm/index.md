---
title: Editing Loading and Background Screens
author: Shakahn
email: pmanuel@worldnet.att.net
description: >
    A short tutorial explaining how to edit BM files (set loading and
    background screens).
date: 1998-06-27
category: jk
---

Author: Shakahn

Editing JK's background screens is ridiculously easy, yet very few
people have done it, so I guess it is up to me to give back to the JK
editing community and tell you how it's done. Here we go...

**Programs needed:**

  - Bmut (in 2020, I can't find this program anymore, but maybe try JKPaint in 
    [programs](/programs/))
  - Conman (look in [programs](/programs/))
  - a BMP file editor (you can use Microsoft Paint, which is free with
    most PCs that are able to run JK)

**How to do it:**

First of all, the files that control the way the loading screens look
are called BMs. You need to go into Conman and open the Res1hi.GOB (or
Res1low.GOB) in the Resource file in the JK directory. Click on bm.
Extract the BM of your choice to a new directory (Bkbuildload.BM,
Bkmain.BM, Bkloading.BM, Bkmulti.BM, and Bksetup.BM are a few good ones)
and exit Conman. Then go into Bmut. Open up the BM that you extracted
and convert it to a BMP file. Open it up with a BMP editor, and change
it however you want. Then go back into Bmut and create a new BM. Click
on the box that says Include Palette. Insert a converted BMP file and
click Create BM. When Bmut asks you what name to save your new BM under,
type in the name of the original BM. When asked if you want to write
over the existing BM, click Yes. PRESTO\! INSTANT NEW BACKGROUND SCREEN
ART\! But we are not quite done yet. Go into the Resource folder in your
JK directory and create a folder called ui. Inside that folder create a
folder called BM. Put all your BMs in there and launch JK as normal. If
you didn't bungle something, you should see your new screen art. If you
don't see your new art, and you can't figure out what went wrong, try asking
on the forums.

