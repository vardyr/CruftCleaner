# CruftCleaner
> A simple Bash script that deletes files and folders within specified folders based on a maximum age.

Idea from "Mind Performance Hacks" by Ron Hale-Evans
Print ISBN:    978-0-596-10153-4 | ISBN 10:    0-596-10153-8
Ebook ISBN:    978-0-596-15311-3 | ISBN 10:    0-596-15311-2
***

## Usage
This script is designed to be run daily as a cron job to clean a folder containing temporary files, such as web browser downloads, based on a maximum age limit.

## Configuration
Configuration consists of two variables, one for the array containing the list of folders to clean, and a second for the maximum age of files in those folders, in days.

`# Temporary folders to clean based on $maxage. Array in the form of: folders=( "/fsroot/folder1/" "/fsroot/folder2/" )
folders=( "/home/user/tmp/downloads/web/" )`

`# Maximum age of files in days
maxage="3"`

## TODO
* Finish this README. Add usage instructions for *nix and Mac OS X. See http://github.com/guides/readme-formatting
* Finish homepage http://vardyr.github.com/CruftCleaner/index.html
