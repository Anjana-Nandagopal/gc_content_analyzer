DNA GC Content Analyzer
A simple Python script that analyzes a DNA sequence and calculates its base composition and GC content.
What it does
This script takes a real DNA sequence (pulled from NCBI — a fragment of Homo sapiens chromosome 6, GRCh38.p14 Primary Assembly) and:
Counts the total number of bases in the sequence
Counts how many times each base (A, T, G, C) appears
Calculates the GC content — the percentage of the sequence made up of Guanine (G) and Cytosine (C)
GC content is a meaningful metric in biology/bioinformatics — it can indicate things like gene density, DNA stability, and is often used to compare or classify organisms and genomic regions.
Example output
This is the DNA sequence of Homo sapiens chromosome 6, GRCh38.p14 Primary Assembly
14084
There are 4009 A bases
There are 2755 C bases
There are 4406 T bases
There are 2912 G bases
The total GC content is 40 %
How it works
The DNA sequence is stored as a multi-line string and cleaned using .replace("\n", "") to remove line breaks copied over from the NCBI FASTA format
Python's built-in .count() string method tallies each base
GC content is calculated using the formula: GC content = (G count + C count) / total length × 100
Requirements
Python 3
Running it
python3 final.py
Possible next steps
Visualize base composition with a bar chart (matplotlib)
Identify the most frequent base programmatically
Search the sequence for specific motifs (e.g., the start codon ATG)
Allow the user to input their own DNA sequence
About
Built while learning Python fundamentals (strings, numbers, lists) and applying them to a real bioinformatics dataset.
