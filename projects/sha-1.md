---
layout: project
type: project
published: true
image: images/sha-1-project-cover.png
title: SHA - 1
permalink: projects/sha-1
# All dates must be YYYY-MM-DD format!
date: 2018-04-30
labels:
  - C
  - Security
  - Encryption
summary: Reconstructed Secure Hashing Algorithm 1 from the white paper.
---

 <img class="ui image" src="../images/code-constants.PNG">
 
## My Role
The goal was to create the hashing algorithm and then to test it on the three provided files. The provided files were three test cases that each tested the algorithm in a different way. Recreating the no longer used encryption algorithm was intended to give greater understanding of not only C but for encryption as well. The bit shifting behind the algorithm (see picture below) was already given as well as a general road map that was provided to assist in understanding what the code was trying to do. This was extremely helpful once I got on the right track.

## The Difficulties

* File reading - C does not always play nice when accessing or exiting files. Setting the required file and open and close parameters was tedious, as if anything was left out you are left in the dark if the file had been corrupted or not.
* Helper Functions - To keep the already large block of code as compact as possible it was necessary to create many helper functions. The problem being was being in this mindset lead to a lot of time wasted in making to many helper functions.
* Hex Values Vs. Char Values - The code relied on the fact that after the file was read in, an end of line character would be the last character. The code was looking for its HEX value not the actual end of line character.
* Getting Lost- With the program being of decent size and with many  moving parts the code is easy to get lost in.

<img class="ui image" src="../images/code-bitshifting.PNG">

## My Solution

* To begin I needed to ensure that the opening/closing of the file be the first thing and the last thing that is done every time the code is run. I started off by feeding it the test case files and appending a string at the end to make sure it was writing to the file. Then I made sure to just open and close each file with getting any issues. Then I went and added helpful error messages to see if the file was opening and closing.

* Helper functions are a good tool. After going a bit overboard with making helper functions I took a critical look at which ones were actually called more than once and removed the rest. Any function that was only called once was hard coded into the program.

* Rather than introduce more variables the end of lines character's hex value was manually added to the array that held the characters that were read in from the file.

* Detailed, relevant, and specific comments were an absolute must. Not having them initially lead to a lot of lost time trying to remember what went where. The almost gratuitous amount of comments paid dividends when I ended up being a peer mentor and other students asked for assistance for this class and about this project in particular.

[Source](https://github.com/pmccrind/secure-hash-1)
