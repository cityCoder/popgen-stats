#popgen-stats

Scripts to calculate population genetics statistics

##selectionStats.py
This script calculates diversity and selection statistics for fasta alignments. Alignments must represent in frame coding sequences. The script will calculate theta, pi, piN, piS, and Tajima's D. If an outgroup(s) is provided, results of the McDonald Kreitman test will also be output. A single fasta alignment or a directory of fasta alignments can be provided to the program.

Requirements: EggLib with Bio++ (http://egglib.sourceforge.net/)

Current Versions: Python v 2.7.3, EggLib v 2.1.7, Bio++ v 2.1.0

Usage:
selectionStats.py -a [alignment] -d [directory] -o ["list, of, outgroups"]

##selectionStatsPlot.R
This script plots the results of selectionStats.py

Requirements: ggplot2 (http://ggplot2.org/)

Current Versions: R v 3.0.2, ggplot2 v 0.9.3.1

Usage:
selectionStatsPlot.R [input filename]