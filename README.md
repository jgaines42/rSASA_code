# rSASA_code

Code for calculating rSASA for amino acids in proteins. rSASA values range from 0 (fully buried) to 1 (as exposed as a dipeptide). 

See details of code and cite  "J. C. Gaines, S. Acebes, A. Virrueta, M. Butler, L. Regan, and C. S. O'Hern, Comparing side chain packing in soluble proteins, protein-protein interfaces, and transmembrane proteins, Proteins: Structure, Function, and Bioinformatics 86 (2018) 581"

Install Naccess from http://wolf.bms.umist.ac.uk/naccess/ \
Then run the code from the same folder

run_Naccess(pdb_folder, pdb_name, save_folder)\
Input: 
pdb_folder: full path the folder with \*.mat file of the pdb. End path
name with / \
pdb_name: Name of the pdb \
save_folder: full path to folder to save results in. End path name with / \

Output: \
\*_sasa_data.mat: contains the following columns: \
   1: Residue id \
   2: rSASA \
   3: SASA of residue in context of protein \
   4: SASA in context of dipeptide (Ca,C,O of prior amino acid and N,Ca, H of next amino acid)\
 
