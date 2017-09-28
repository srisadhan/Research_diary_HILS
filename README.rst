calliope
--------
A simple script that makes it easy to use LaTeX for journal keeping - most useful for keeping research journals!

This script is based on the original project here: https://github.com/mikhailklassen/research-diary-project - do take a look!

The name
========

`In Greeky mythology, Calliope is the muse that presides over eloquence and epic poetry. <https://en.wikipedia.org/wiki/Calliope>`__

Epic poetry is exactly what our private research journals are ;)

Requirements
============

- latexmk
- pdflatex
- makeindex
- packages used in templates/research_diary.sty

.. code:: bash

    sudo dnf install 'tex(opensans.sty)' 'tex(framed.sty)' 'tex(multirow.sty)' 'tex(wrapfig.sty)' 'tex(booktabs.sty)' 'tex(makeidx.sty)' 'tex(listings.sty)' latexmk /usr/bin/biber 'tex(biblatex.sty)'

Tested on a Fedora 24 Linux system, and should work on most Linux variants.

Usage
=====

.. code:: bash

    usage: ./calliope.sh options

    Master script file that provides functions to maintain a journal using LaTeX.

    OPTIONS:
    -h  Show this message and quit

    -t  Add new entry for today

    -l  Compile latest entry

    -c  Compile today's entry

    -a  <year>
        Year to generate anthology of

    -p  <year>
        Compile all entries in this year

    -s  <entry> (yyyy-mm-dd)
        Compile specific entry


NOTE: Please grep the various template files for my name and replace it with yours before you begin.
