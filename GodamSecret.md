# SKR CTF: Godam Secrets
*Cylroth created this page on Dec 1, 2024*

## Description
We managed to recover part of Godam's hard drive in his house, but we couldn't find anything suspicious. We hope you can help us in finding his secret.

## Hints
1. Where does Firefox history stores at?
2. Visit [here](https://sqliteonline.com/) to open sqlite file

## Files
**godam_hard_drive.zip**

## Solution
### Recon
- Seem to be having a sqlite file in the zip file.
### Execution
To begin with, I unzip the file using `unzip godam_hard_drive.zip` .After that, "home" file will be created in the directory. According to the first hint, I found that Firefox history store at "profile" directory. I'm redirecting my directory using `cd home/godam/.mozilla/firefox/profile/` (The address is copied from unzip command process)


