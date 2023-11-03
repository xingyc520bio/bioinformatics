## Exercise 3: A more complex sequence analysis example.
### part 1
The example sequence in this case is called ***NCK1_HUMAN***. 
Find it using the search box at the SWISSPROT database (as in Exercise 2). 
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/ea356b65-0427-4c70-8de2-15476b3516a6)

Again save the sequence in a text file (you will need it again later).           

```fasta
>sp|P16333|NCK1_HUMAN Cytoplasmic protein NCK1 OS=Homo sapiens OX=9606 GN=NCK1 PE=1 SV=1
MAEEVVVVAKFDYVAQQEQELDIKKNERLWLLDDSKSWWRVRNSMNKTGFVPSNYVERKN
SARKASIVKNLKDTLGIGKVKRKPSVPDSASPADDSFVDPGERLYDLNMPAYVKFNYMAE
REDELSLIKGTKVIVMEKCSDGWWRGSYNGQVGWFPSNYVTEEGDSPLGDHVGSLSEKLA
AVVNNLNTGQVLHVVQALYPFSSSNDEELNFEKGDVMDVIEKPENDPEWWKCRKINGMVG
LVPKNYVTVMQNNPLTSGLEPSPPQCDYIRPSLTGKFAGNPWYYGKVTRHQAEMALNERG
HEGDFLIRDSESSPNDFSVSLKAQGKNKHFKVQLKETVYCIGQRKFSTMEELVEHYKKAP
IFTSEQGEKLYLVKHLS
```

![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/d71a07fd-9bac-4296-9921-df607f97330d)


We are going to try to find out something about the likely structure and function of this sequence on the basis of similarity to database sequences.

### Part 2. Run a FASTA search at the NPS@ server. 

(tip: paste just the sequence into the box - without the header information)
Link is: https://npsa-pbil.ibcp.fr/cgi-bin/npsa_automat.pl?page=/NPSA/npsa_server.html   

![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/51a0e74a-8335-4970-a695-031774204e10)

Examine your results. 

![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/44efb6ab-811e-46f5-a9e5-67c41141f0bf)

You will see that the very protein itself is within SWISSPROT, and found, unsurprisingly, as the top hit. However, we'll ignore this for the moment and imagine a more realistic situation where this is not the case. 
This amounts to learning about the query protein using hits from the second best onwards.

![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/94aa4306-c30f-440c-9e8f-1688638d3353)

Looking at the list of hits we don't see one dominant type of hit as we did with the glutathione S-transferase sequence. 
We see some tyrosine kinases, some phosphatases, some GTPase activating proteins, and some others. 
This would lead us to suspect that our protein has some role in signal transduction, but tells us nothing more specific.

Within the top ten hits is GRAP_DROME (Q08012). 
Click on the e-value (right-hand column) and examine the alignment. 
There are two very striking features in this alignment. 
What do you think they are? 
What might they tell us about the domain structure of our query sequence, and about its likely functional similarity with DRK_DROME? 
Scroll down a few more alignments and see if you can learn any more.

### Part 3. Re-do part 1 but this time use blastp at the NPS@ server.

Note that blast often reports several segments of similarity between each pair of sequences 
(click on the link from the E-value on the results page to get the alignment). 

```python
MAEEVVVVAKFDYVAQQEQELDIKKNERLWLLDDSKSWWRVRNSMNKTGFVPSNYVERKN
SARKASIVKNLKDTLGIGKVKRKPSVPDSASPADDSFVDPGERLYDLNMPAYVKFNYMAE
REDELSLIKGTKVIVMEKCSDGWWRGSYNGQVGWFPSNYVTEEGDSPLGDHVGSLSEKLA
AVVNNLNTGQVLHVVQALYPFSSSNDEELNFEKGDVMDVIEKPENDPEWWKCRKINGMVG
LVPKNYVTVMQNNPLTSGLEPSPPQCDYIRPSLTGKFAGNPWYYGKVTRHQAEMALNERG
HEGDFLIRDSESSPNDFSVSLKAQGKNKHFKVQLKETVYCIGQRKFSTMEELVEHYKKAP
IFTSEQGEKLYLVKHLS
```
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/151ab526-d0f8-4b28-8a88-87a7a96208e9)

Do you find it easier to deduce the domain organisation from this output than from that of fasta? 
If you are unsure ask a demonstrator.
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/2debc66e-ed5e-4d81-9027-a8fb23c7c0b0)

![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/5d6bfbbd-6608-4eb5-8d0f-a40dff18e069)

BLASTp take a little bit longer and it have lower e-value and higher sensitivity.


