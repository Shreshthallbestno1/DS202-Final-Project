# dbwt
dbwt downloaded from https://code.google.com/archive/p/csalib/downloads

in the ```dbwt``` folder, run 
```bash
make
```

Citing dbwt README File - \
Direct BWT construction

Kunihiko Sadakane
National Institute of Informatics (NII)
sada@nii.ac.jp
http://researchmap.jp/sada/

Usage:

dbwt filename
  compute the BWT of the file "filename".  Output files are "output.bw" and
  "output.lst" (the rank of the last character).
  The output files can be used for csalib.

Limitation:
  The program will work only if the input file is of size < 4GB.

Acknowledgment:
  The file "sais.c" was written by Yuta Mori.
  http://sites.google.com/site/yuta256/

Algorithm:
  This program is based on the algorithm proposed in
    Daisuke Okanohara, Kunihiko Sadakane. A Linear-Time Burrows-Wheeler Transform 
    Using Induced Sorting. In Proc. of SPIRE, LNCS 5721, pp. 90-101, 2009,
  with some simplification.  For most of inputs, the program uses less than 2.5n bytes
  where n is the length of the input.

Changes:
2010-07-30: Fixed a bug (the previous one did not work on Ubuntu).
2010-07-17: First release.

# libdivsufsort
libdivsufsort cloned from https://github.com/y-256/libdivsufsort.git
```bash
git clone https://github.com/y-256/libdivsufsort.git
```
The following assumes it was cloned in a folder called ```libdivsufsort```

# Running
For the reasons of large storage space required, the original database is not included. The ```database.xlxs``` contains all the database details and sources used to gather the data.

After downloading the data, store them in respective folders under ```./Datasets``` folder. Eg. Store english corpus into the ```./Datasets/english``` folder, and so on.

The file ```runBWT.ipynb``` contains all code to run and plot the graphs.

Final graphs and data table are present in ```./Datasets/Output``` folder

## Requirments to run the notebook
Other than standard python libraries, following are needed:\
Numpy\
Matplotlib\
Pandas\
