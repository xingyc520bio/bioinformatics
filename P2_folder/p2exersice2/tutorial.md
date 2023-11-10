# Exercise 2. The dnaJ domain.
You might remember the dnaJ domain from the previous practical. 
We're going to use it again this week to consider how to use structural information in making multiple alignments. 
An important thing to remember when making multiple alignments is that the sequences MUST have the same domain organisation. 
The BLAST searches we did last time revealed lots of proteins from Arabidopsis and S. Cerevisiae that contain a J domain but are otherwise unrelated (apparently). 
We will try to align some of these dnaJ domains. The structure of dnaJ from E. Coli has been determined by NMR and is in the PDB file 1xbl.pdb.
You can use Pymol to take a look at the structure of this small domain, as described below. 
Alternatively, go to the PDB site and find 1xbl entry and select 3D view: Structure on the left panel. 
To start Pymol, first start the AppsAnywhere Portal, wait for validation, and then find and start Pymol.
the link is:https://appsanywhere.leeds.ac.uk/
Click on File, then Open to load this file.
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/cfd21a7c-9995-4e8a-85b3-f7f6a96b49f1)

It is an all alpha domain with four helices 
(You may need to switch to JSmol viewer to see that).
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/1f97fab3-d72a-4da6-970d-1fb7c088419c)

The sequences for the dnaJ domain are in dnaj_all.fasta file. 
This file has been produced by manual editing of the real file from SWISSPROT to remove parts of the sequence which are not the dnaJ domain. 
All this editing of sequence files can be tedious, but it is essential. 
Download the dnaj_all.fasta file and analyse it with Clustal Omega server from the previous example. 
Download the alignment and view it with the JalView. 
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/1106a5f5-ade4-471e-a3a5-e67580df8c14)

##### Does the alignment of a single domain make more sense? 
Yes, maybe it is an important domian which have important fuction.

##### Can you relate the alignment with the 3D structure?
The best alignment is from the alpha-helix binding the small molecular.
