# User Guide: Phage Annotation with PHASTEST https://phastest.ca/

## 1. Input method
PHASTEST accepts inputs in 3 formats: GenBank annotations, raw nucleotide sequences, and FASTA-formatted nucleotide sequences.

The program runs the fastest with pre-annotated GenBank inputs, but as the name totes, it will ultimately run relatively quickly regardless of input format.

- If using a GenBank input you can upload the GenBank-formatted file on the "Upload File" tab, or you can enter the GenBank accession number on the "Enter GenBank Accession" tab and PHASTEST will fetch the annotation for you.

- If using a raw nucleotide sequence, your only option is to paste the raw text directly on the "Paste Sequence" tab.

- If using a FASTA-formatted nucleotide sequence, you can upload the FASTA file on the "Upload File tab, or you can paste the sequence directly on the "Paste Sequence" tab.
   - If your FASTA file contains multiple contigs (multi-FASTA), you must use the "Upload File" tab and check the box that says "My input consists of multiple separate contigs".

## Other input parameters
### Bacterial sequence annotation mode
Regardless of your input format, PHASTEST will ask that you choose between "Lite" and "Deep" annotation modes.

Lite annotation uses the Swissprot database, and makes the program run faster.

Deep annotation uses PHAST-DSB (PHASTEST Bacterial Sequence Database), and makes the program run slower.

Deep annotation is more accurate than lite annotation in that it misses fewer proteins, but it is up to you to choose whether you are looking for high speed or high accuracy. For some inputs, lite annotation returns results comparable to those produced by deep annotation, but for other inputs, deep annotation is significantly better at predicting proteins (see Table 6 on https://phastest.ca/statistics).
