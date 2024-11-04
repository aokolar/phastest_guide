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
At the bottom of the input window is a pre-checked box that says "Remember My Searches". If you leave this box checked, PHASTEST will remember any annotations you run in your current browser. This option uses cookies to remember your information.

To access your previously completed searches, click on the three parallel lines in the top left corner of any page, then navigate to "My Searches". 

If at any time you want to remove a result from your saved searches, open that search's results page and uncheck the "Remember Me" box in the top right corner of the page.

## When you are ready, click "SUBMIT" and let PHASTEST work its magic.

## 3. Submission results
If you wish to download a .zip file of your annotation results, you can do so by clicking the link next to "Download Results" at the top of your submission results page.

### 3.1. Region summary
This tab shows an overview of any and all potential phages that were found in your input sequence. This page also gives some details on what type of phages were found, how complete their genetic information is, and where they are located in the bacterial genome. All of this information is explained directly on the page.
![image](https://github.com/user-attachments/assets/035d37b9-a1cd-4e94-aa47-a7b962df5e68)

### 3.2. Phage genes
This tab shows what kinds of phage genes were found in your annotation, where they are located, and how confident PHASTEST is in their correctness. Results are color-coded by the functions of their encoded proteins, with a color legend given at the top of this page.
![image](https://github.com/user-attachments/assets/2c3c20e5-059f-4641-857f-6a92b3fbff46)

### 3.3. Bacterial genes
This tab functions the same as the "phage genes" tab, but shows the bacterium's annotated genes instead. This tab's results are also color-coded, but there are much fewer categories that PHASTEST puts these genes in, since the program is geared towards phages after all. This tab might be useful for quick reference, but I wouldn't recommend using PHASTEST as your go-to tool for whole-genome annotation.
![image](https://github.com/user-attachments/assets/d208cfa7-f2a3-491a-93e8-bd86e0e0536b)

### 3.4 Genome viewer 2.0
