## Exercise 2: Similarity searches for glutathione S-transferases.
This exercise involves searching for sequences similar to ***glutathione S-transferases*** within the SWISSPROT database. 
These proteins form a large and rather diverse family. 
Goto the ***SWISSPROT database*** .      
Link is: https://www.uniprot.org/
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/d4040f68-2e42-44d9-a5ff-c7e7cbd71e18)

Use the search box to find hits to ***human glutathione S-transferase*** go and view the entry P09488 from the list. 
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/9ed0f6d6-c91f-4d48-8315-c7faf21c1946)



Scroll down to the Sequence Information section and click on ***FASTA format***. 
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/be824056-8ab0-4fac-9b22-72f6d00f1756)


This is the query sequence (in FASTA format). Highlight the sequence then select Copy from the browsers Edit menu. Paste the sequence into a text file (e.g. use Notepad for this) in your home directory (M:\ drive) , 
and save it as a text file to a filename you can remember *e.g. P09488.fasta*.

![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/68a58bf9-a295-4302-b4e5-ec52bf87a2ba)


### Part 1. Run a preliminary search using the fasta algorithm.

Goto the ***EBI FASTA*** server.     
Link is: https://www.ebi.ac.uk/Tools/sss/fasta/
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/9f6f60f9-6669-45f1-8210-1c7ff4049778)



On the submission form choose the swiss-prot database and request 150 scores and 150 alignments (click "More options"). 
Then either paste the FASTA format sequence into the box or upload the file you saved using the "Browse.." option, and press Submit.
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/044a06cb-8e19-40ac-b64c-6d105e4a0aca)

Examine the results file. Examine your significant hits (lets take a cutoff at E=0.001 to define significance for the purposes of this exercise). 
Note that most significant hits are indeed glutathione S-transferases. But note also that some glutathione S-transferases do not have significant scores, 
showing that simple pairwise comparison is not always sufficient to detect an evolutionary relationship. 

I get this email   
The results for the job "Miss Xing" (ID: fasta-E20231103-140303-0703-59897707-p1m) can be viewed at:    

http://www.ebi.ac.uk/Tools/services/web/toolresult.ebi?tool=fasta&jobId=fasta-E20231103-140303-0703-59897707-p1m

The job results will be available for 7 days.
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/acf838f2-99a3-499d-b4d7-64cb22243d25)


Note also that a protein called S-CRYSTALLIN generates significant scores. These are not glutathione S-transferases, 
in fact these proteins are believed to play a structural role in the eye lens. They are not even enzymes. What does this tell us about evolution, 
and the use of sequence similarity to predict function?

# Part 2. Run the same search using the Smith-Waterman algorithm SSEARCH server at the EBI

and proceed as before.

Again choose the ***swiss-prot database***.      
Link is: http://www.ebi.ac.uk/Tools/services/web/toolform.ebi?tool=fasta&program=ssearch&context=protein     

And request 150 scores and 150 alignments (Click "More options"). 
Then paste the FASTA format sequence into the box, and press Run. Notice how much slower it is than fasta. 
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/2ed57d37-96e7-4c92-ac36-a1ffb4e7ad8a)

Examine your results. 
![image](https://github.com/xingyc520bio/bioinformatics/assets/49332831/8f7ac84d-6665-411c-802a-7659b3ed5c07)

*Is there any difference?*    

E values are different. swith waterman have lower E value and higher similatity so it is more sensitive.
