---
layout: default
title: "SNHU CS-Portfolio"
description: Software Design and Engineering
---


# Software Design and Engineering Enhancement

Before I combined both projects, I was performing a considerable amount of
cleanup work on the two projects.

The reason I combined them is due to the similarities between projects.
Both used a list-like structure and displayed an object with two strings.

The new goal was to take the original Jukebox concept and the Playlist UI
and combine them.

The first part:
1. **External database** to allow growth and changes to playlists. **(MongoDB)**
2. **Skipping** songs and replaying songs,
3. Ability to **change** playlists **during playback** (text playback).

After core functionality is implemented, I added smaller features to the
UI.


These goals were accomplished, though I had hoped to include personalization
and custom playlists.


> How each slide is made after implementing this class.

``` java
/**
 * Constructor for a slide
 *
 * @param   str1        The title of a slide
 * @param   str2        The description of a slide
 * @param   imagePath   Path to the image
 */
public Slide(String str1, String str2, String imagePath) {
    this.str1 = str1;
    this.str2 = str2;
    this.imagePath = imagePath;
}
```


After I expanded on this idea, I used the slideshow UI template to plug in
the strings I needed. It started out looking like this, and the end result
is almost identical. (It's Java.awt and Swing)

<div style="color:white; display: inline-flex;">

<svg><rect fill=white width=128 height=128></rect><rect fill=black width=100 height=64 x=12 y=12 ></rect><rect fill=black width=100 height=4 y=84 x=12></rect><rect fill=black width=100 height=4 y=94 x=12></rect><rect fill=blue width=40 height=18 x=16 y=104></rect><rect fill=red width=40 height=18 x=68 y=104></rect></svg>
White box -> application<br>
Large black rectangle -> the image<br>
First thin line -> artist<br>
Second thin line -> song title<br>
Left Blue Button -> previous button<br>
Right Blue Button -> next button<br>
</div>


<a href="/" class="btn">Return Home<a>
