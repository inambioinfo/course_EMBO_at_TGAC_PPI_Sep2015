---
title: MSA & Jalview
layout: page
---

In these exercises, we will introduce and work with Jalview the JAVA Alignment Viewer. Jalview is powerful visualisation software that can allow alignments to be generated, manipulated, edited and annotated. It interfaces remotely with tools such as multiple sequence alignment programs and secondary structure predictors. We will visualise alignments of modular proteins with Jalview, discussing sequence features such as folded protein domains, short functional peptide motifs and natively disordered polypeptide. These structure-function modules will reappear regularly during the course.

The JalView developers are now making training videos for YouTube. You can access these at the The JalView Youtube channel.

Part 1. Using Jalview with Epsins
=================================

-   Go to the Jalview downloads page and choose "Launch Jalview Desktop"
-   Load a set of sequences by cut and paste into Jalview using:
-   File-\>Input Alignment-\> from Text Box
-   Cut the sequences from this page of Epsin Sequences in FASTA format
-   Remotely align sequences via the Web Service-\>Alignment-\> options (Choose a service and run with defaults)
-   Different participants can do the alignment using different MSA tools so we can compare the results afterwards
-   Examine the alignment, identify possible regions of misalignment, and try correcting these by moving bits of sequence as described in the Jalview documentation; remember to Select-\>Deselect All if you are unable to make the edits you want
-   Get a remote secondary structure prediction by the JNet surver using the Web Service link
-   Look at the conservation of DPW, NPF, and clathrin boxes using Select-\>Find...-\> providing the appropriate text pattern, and doing Find All
-   Follow this up by creating and naming a New Feature from the pattern matches
-   Save the annotated alignment data in a file in Jalview format - this allows you to examine in the future these and other features/annotations you may add to your alignment File-\>Save As-\>FileFormat Jalview (.jar)
-   Sort the order of sequences in the alignment, clustering by pairwise identity Calculate-\>Sort-\>By Pairwise Identity

Questions:
----------

1.  What is the basis for the "ClustalX" colouring scheme provided by Jalview?
    1.  which residues are assigned similar colours?
    2.  which residues are assigned different colours?
    3.  in which situations are residues left uncoloured?
    4.  Try some other colouring schemes.

2.  Are matches to the linear motif regular expressions more likely to be conserved in regions known/predicted to be globular or in IUP regions? Does the JNet 2D structure predictor suggest large numbers of alpha helices and beta strands throughout the alignment?
3.  What are the characteristics of regions of the MSA that you expect to be well aligned? Consider:
    1.  residue identity/property conservation
    2.  number and size of gaps

4.  Would you expect the affinity of a domain - linear motif interaction to be higher or lower than one between two domains?
    1.  Why?
    2.  What assumptions are you making about the nature of these different kinds of interactions?

Part 2. Using Jalview with p53s
===============================

Try a similar exercise yourself using p53 sequences (perhaps using this linked set of unaligned p53 sequences). Search in the sequences and make new features with different colours for the following motifs:

-   Cyclin box
-   SUMO modification site
-   MDM2-interaction motif

Questions:
----------

1.  Some of the sequences included in the MSA are shorter than others. Why might this be? Do all sequences begin with a Met residue? If you want a high quality alignment, will you keep these sequences or discard them?
2.  Do all p53 sequences have MDM2 interaction motifs? Have they all been found by the motif pattern? Is there a way to improve the pattern?
3.  Do all p53 sequences have cyclin box candidates? Are they all in the same place in the sequences?
4.  Do all P53 sequences have SUMO sites? Can they all be aligned? If not, is there an evolutionary process that can account for their change in position?

Part 3. Using Jalview with TIR protein isolates from pathogenic E. coli
=======================================================================

TIR proteins are secreted by pathogenic E. coli. They attach to targeted mammalian cells and the N- and C- termini enter through the membrane, taking over the local cell regulation and, with other inserted proteins, induce the actin pedestal. The central portion of TIR remains extracellular and is bound by the bacterium. Many TIR isolates have been sequenced and are in Uniprot.

-   Load by cut and paste this already aligned set of TIR proteins into Jalview.
-   Go to the ELM server that you have just been using and find the Cyclin and CDK motif entries and use the regular expressions to create new features in all sequences.
-   Do all sequences have both motifs?
-   Are they all alignable, or can they move around?
-   Some are juxtaposed - can they both be functional at the same time?
-   Note that as far as we know in creating this exercise, these motifs have not been studied, but there is some evidence that cell cycle is disrupted by pathogenic E. coli (e.g. PMID: 11598051). Pathogens might commonly secrete into the cells that they take over proteins that are natively disordered and contain linear motifs to control cell regulation.

Publications
============

Jalview Version 2--a multiple sequence alignment editor and analysis workbench. Waterhouse AM, Procter JB, Martin DM, Clamp M, Barton GJ. Bioinformatics. 2009 May 1;25(9):1189-91. PMID: 19151095

Fast, scalable generation of high-quality protein multiple sequence alignments using Clustal Omega. Sievers F, Wilm A, Dineen D, Gibson TJ, Karplus K, Li W, Lopez R, McWilliam H, Remmert M, Soeding J, Thompson JD, Higgins DG. Mol Syst Biol. 2011 Oct 11;7:539. PMID: 21988835