ZK stats extracted from The Archive.

Quick Start

Install dependencies python3 pip3 install pandas plotly
Adjust user setting section
Then run the script via the command line python3 ogden.py
Details

If you do not use a prepended symbol to signify UUIDs, don't worry. Just leave the variable alone. Removing it will cause an error.
This script assumes you are including the date in the format of yearmonthday in the note names. It won't matter the position of the date in the file name. - For links, the script assumes and counts [[wikilinks]] that contain at least the date and time string of the linked-to note. The link can contain the title of the note or not. It will count multiple links on a line.
For links, the script will not count [["bracket tags"]] as a link. The type of links it does report are:
1. [[202109291617]] - UID only links
2. [[202109291617 Stats Python Script]]
3. [[Stats Python Script 202109291617]]
4. ›[[202109291617]]‹ - which are interstitial non note oriented
      (you probably don't have any of theses and don't worry)
      (if you want other link formats, please let me know)
Assumes all notes are in the same folder. It does not care if they are .md or .txt as long as they have the UID in the form of yearmonthday...
The stats.csv file (location set in the user settings) is the file used by the graphing function. It is <100k and can be safely placed anywhere. It might be good to place it in your downloads directory, where you can easily find it for review or troubleshooting.
You can comment out any of the graphs you don't want.
Don't hesitate to get in touch with me through the forums at @Will https://forum.zettelkasten.de/discussion/1964/exposing-the-zettelkasten-to-the-quantitative-eye
Further discussion and help is avaiable.