---
layout: default
---
***
Idea from "Mind Performance Hacks" by Ron Hale-Evans, "Pre-Delete Cruft" (Hack #18, p.67)  
*Print ISBN:    978-0-596-10153-4 | ISBN 10:    0-596-10153-8*  
*Ebook ISBN:    978-0-596-15311-3 | ISBN 10:    0-596-15311-2*  

## About
Inspired by a chapter in the book "Mind Performance Hacks" by Ron Hale-Evans entitled "Pre-Delete Cruft" (Hack #18, p.67), I began thinking of ways to pre-delete cruft.

Cruft, in a general sense, is "[any accumulation of obsolete, redundant, irrelevant, or unnecessary information, especially code](http://en.wikipedia.org/wiki/Cruft)." I will leave full exploration of the reasons for pre-deleting cruft as well as how to separate the cruft from important information to the author of the book.

The most obvious example of cruft on a networked computer is in the form of web browser downloads. Most of the time, a user downloads a file, opens it, and never uses it again after opening it that first time. This is especially true in the case of program installers; by the time the installer is needed again, it is often outdated.

In a folder full of five hundred downloaded files, it can be time-consuming to find the one file you're looking for. Modern browsers feature a download manager, but if you've cleared the item out already you could need search for the file or browse to your downloads folder and sort by date. This is extra work to sort through needless clutter.

Modern operating systems feature powerful search functions for the express purpose of finding specific information amidst heaps of clutter. These tools are limited, however; a multitude of similar filenames can seriously impact the efficiency of searching. If a user organizes files in a logical and sensible manner, while deleting cruft regularly, these tools become supplemental rather than absolutely necessary. Additionally, these tools introduce a measure of overhead, consuming CPU cycles, memory, and precious battery power indexing and searching through a significant amount of data that probably should've been deleted ages ago.

Think you might want to keep a file? Simply save it elsewhere. This script is intended to clean folders containing transitory, disposable files.

## Usage
This script is designed to be run daily as a cron job to clean a folder containing temporary files, such as browser downloads, based on a maximum age limit.

## Configuration
Configuration consists of two variables, one for the array containing the list of folders to clean, and a second for the maximum age of files in those folders, in days.

    # Temporary folders to clean based on $maxage.
    #   Array in the form of: folders=( "/fsroot/folder1/" "/fsroot/folder2/" )
    folders=( "/home/user/tmp/downloads/web/" )

    # Maximum age of files in days
    maxage="3"