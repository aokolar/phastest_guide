# User Guide: Phage Annotation with PHASTEST https://phastest.ca/

## 1. Input method
PHASTEST accepts inputs in 3 formats: GenBank annotations, raw nucleotide sequences, and FASTA-formatted nucleotide sequences.

The program runs the fastest with pre-annotated GenBank inputs, but as the name totes, it will ultimately run relatively quickly regardless of your input format.

- If using a GenBank input, you can upload the GenBank-formatted file on the "Upload File" tab, or you can enter the GenBank accession number on the "Enter GenBank Accession" tab and PHASTEST will fetch the annotation for you.

- If using a raw nucleotide sequence, your only option is to paste the raw text directly on the "Paste Sequence" tab.

- If using a FASTA-formatted nucleotide sequence, you can upload the FASTA file on the "Upload File" tab, or you can paste the sequence directly on the "Paste Sequence" tab.
   - If your FASTA file contains multiple contigs (multi-FASTA), you must use the "Upload File" tab and check the box that says "My input consists of multiple separate contigs".

## 2. Other input parameters
### 2.1. Bacterial sequence annotation mode
Regardless of your input format, PHASTEST will ask that you choose between "Lite" and "Deep" annotation modes.

- Lite annotation uses the Swissprot database, and makes the program run faster.

- Deep annotation uses PHAST-BSD (PHASTEST Bacterial Sequence Database), and makes the program run slower.

Deep annotation is more accurate than lite annotation in that it misses fewer proteins, but it is up to you to choose whether you are looking for high speed or high accuracy. For some inputs, lite annotation returns results comparable to those produced by deep annotation, but for other inputs, deep annotation is significantly better at predicting proteins (see Table 6 on https://phastest.ca/statistics).

### 2.2. Pre-computed results
If you are submitting your input from the "Upload File" or "Paste Sequence" tabs, PHASTEST automatically checks a box that says "Use pre-computed results if available".

- If you leave this box checked, PHASTEST can retrieve existing results for your input query: for example, if you uploaded a GenBank file that someone else had previously run through PHASTEST, the program will return those results to you rather than redoing the entire annotation. If preexisting results exist for your input, this will save you some time.

- If you uncheck this box, PHASTEST will not retrieve existing results, and will run your annotation from square one.

### 2.3. Email notification
Regardless of your input method, PHASTEST gives you a text box where you can input your email address to be notified when your annotation is done processing. This is not mandatory, especially because PHASTEST completes an annotation within a few minutes, but I highly recommend entering your email if you want to save your results for later! The URL for your results page never expires, so you can keep the link for future reference and your results will still be there.

### 2.4. Remember me
At the bottom of the input window is a pre-checked box that says "Remember My Searches". If you leave this box checked, PHASTEST will remember any annotations you run in your current browser. This option uses cookies.

To access your previously completed searches, click on the three parallel lines in the top left corner of any page, then navigate to "My Searches". 

If at any time you want to remove a result from your saved searches, open the results page and uncheck the "Remember Me" box in the top right corner of the page.

## When you are ready, click "SUBMIT" and let PHASTEST work its magic.

## 3. Submission results
### 3.1. Region summary

### 3.2. Phage genes

### 3.3. Bacterial genes

### 3.4 Genome viewer 2.0
