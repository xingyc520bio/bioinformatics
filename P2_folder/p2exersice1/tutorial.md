# Exercise 1: Multiple alignments of the serine-threonine dehydratase domain
In this exercise you will make a **multiple alignment** of a number of serine-threonine dehydratase (STD) domain sequences. 
The alignment will be created with the Clustal Omega program at the EBI. We will then view the results using a JAVA graphical interface called JalView.

The sequences are given in fasta format in the file stdehyd.fasta. 
The first step is to run Clustal Omega (using the default parameters) at the EBI. 
link: https://www.ebi.ac.uk/Tools/msa/clustalo/
Rather than pasting in your sequences you should upload the file containing the multiple sequences using the "Browse..." button at the bottom of the form.

Then press Submit.
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/cebda658-0ad6-43de-9435-0b12e60ac0fc)

When the alignment is complete, switch to Results Viewers tab. 
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/796ebd5c-7b00-4fc9-ab22-7aa65d533553)

To use the JalView, 
we first need to install it. Click on "free installation are available" and select Jalview executable .jar file (the last). 
It will download and start the Jalview program. Close all the tabs opened in the Jalview program. 
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/69b6feeb-f8db-4c84-97ee-0a8f80d36247)
The url is http://www.ebi.ac.uk/Tools/services/rest/clustalo/result/clustalo-I20231110-144257-0983-60070185-p1m/aln-clustal_num
Open your alignment in the Jalview. For that either save your alignment as a file and open it, or copy and past the corresponding url.
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/f1ce2a3c-8291-4d1b-b2be-7126f6bac581)

Increase the window size by dragging the window down until you have all the sequences in view. 
Use the scrollbar to browse along the alignment. 
What do you think, is it good or bad? 
I think the higher the conservation is, the better the aliment is.
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/080d5fdb-1ab0-4b34-bb86-73b4868bba34)

You will notice that this is a large domain and the sequence set is quite diverse.

JalView gives us the facility to make manual edits to the alignments. 
But it only allows the insertion or removal of gaps (denoted by "-"). 
You can do this by holding down the shift key and selecting a residue with the mouse and dragging that residue left or right. 
Gaps are automatically inserted/deleted but non-gap residues can not be overwritten.

Practise making edits to the alignment. 
In this case, in the absence of structural information, it is quite hard to improve the alignment. 
You can see how well you are doing by clicking on Colour on the menu bar and choosing the Percentage Identity colour scheme this will automatically update the alignment match. 
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/6e0a9f4a-192f-4d7f-bf6a-d6f7dc0c5756)



Its not easy to get a better looking alignment is it? 
By now you might have made a bit of a mess of the original alignment. 
Use the undo facility (Ctrl-Z) to restore the alignment.

Click on the Calculate-> 
Calculate Tree or PCA on the menu bar and choose the Neighbour joining using PID (% identity) menu and this will calculate a tree using Percentage Sequence Identity. 
Have a quick read about this method in the Help->Calculations->Trees and PCA->Calculating trees section then continue.
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/80ca37cd-b698-45c8-a9aa-e91d0e23a8a6)

In the window containing the tree right click the mouse. 
This will draw a line and sorts the tree into clades (by using a different color).
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/a3bbb4ca-556f-495d-a75a-212ad6457e20)

Notice that if you click at different parts of the tree branches you will get different (coloured) groupings. 
Notice also that this changes the colours of the sequence names in the main sequence alignment box to reflect the colours of the tree. 
Is the tree biologically sensible?
No.

You could also calculate the tree using the Neighbour joining tree using BLOSOM62 option. 

![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/d73a7e4d-835e-458c-b78f-ac80ac0cbc48)
Does this tree look more reasonable? 
No.

You can explore some other features of JalView e.g. the different colour options (do this in your own time and note that the manual explains various options).

Now calculate the PCA by selecting Calculate-> 
Calculate Tree or PCA ans selecting Principal Component Analysis and pressing Calculate. 

![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/ef81f7d0-dbcf-43f0-be63-1f7d3c412486)

This is another way to represent similarities between the aligned sequences. 
They are grouped in clusters in the 3 dimensional space along the principal components. 
You can use mouse to rotate the components and see the clusters.
