# pmwiki-kate - PmWiki markup syntax highlighter for Kate editor/KatePart

The XML file in this repository (`pmwiki.xml`) contains rules for highlighting the syntax of [PmWiki](http://www.pmwiki.org/) markup files in [Kate](http://kate-editor.org/), the default text editor for [KDE](https://www.kde.org/). This can be helpful if you want to edit wiki pages offline before saving them to PmWiki, and is similar to the existing syntax highlighter for MediaWiki.

Once [installed](#installation), opening any file with the `.pmwiki` extension should automatically highlight PmWiki syntax as in the example below:

![PmWiki syntax highlighting screenshot](https://cloud.githubusercontent.com/assets/9295750/14151653/c4d86610-f663-11e5-90ed-80f0c7fe5a45.png)

This highlighter works fine with Kate or [Kwrite](https://www.kde.org/applications/utilities/kwrite/) (which are both based on [KatePart](http://kate-editor.org/about-katepart/)), and should also work with any version of PmWiki.

## Installation

Steps to install the PmWiki syntax highlighting file:

1. Download the file `pmwiki.xml` or clone this repository
2. Find the folder `~/.kde/share/apps/katepart/syntax/` on your system (create it if it does not already exist)
3. Move `pmwiki.xml` into `~/.kde/share/apps/katepart/syntax/`
4. Open or restart Kate to use the syntax highlighter.

Default syntax highlighting files for Kate are usually stored in the folder `/usr/share/kde4/apps/katepart/syntax/`. However, custom syntax highlighters should probably be saved in the local syntax highlighting folder (`~/.kde/share/apps/katepart/syntax/`) in the user's home directory so that they don't get accidentally overwritten during an update.

## Usage

Files with the extension `.pmwiki` will automatically be highlighted using the rules in `pmwiki.xml`. Plain text or other files can be forced to use PmWiki highlighting rules by selecting _PmWiki_ from the _Highlighting_ menu:

* __Tools__ > __Highlighting__ > __Markup__ > __PmWiki__

## License
Based on [kate-markdown](http://github.com/claes/kate-markdown/) by [Claes Holmerson](http://github.com/claes/).

Dual-licensed under both GPL and BSD licenses.
