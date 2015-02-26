
FD/DH pKa calculation code, Warwicker Lab, Manchester 2011
References
Warwicker (2004) Protein Science
Warwicker (2011) Proteins, submitted

The code and data is available as a tar file.
The files contained are:

for BUILDING the FD/DH code:

.f			fortran files, should be suitable for compilation on 32 bit or 64 bit machines

FDDH_export_build.scr 	script will build the appropriate binaries - just sub in your compiler

for RUNNING FD/DH code:

multi_FDDHpK_export.scr	scripts goes through the complete process from a list of PDBs to pKs for each PDB

FDDHpdb.list		the list of PDBs for calculation with the multi_FDDHpK_export.scr script,
			each PDB (one per line) listed as X.A, mean look for chain A in PDB file X.pdb
example PDBs		the example FDDHpdb.list links to the two 3BDC derived PDBs supplied
			
.in, .ctr, .chr, .dat	files are various standard parameter or dictionary files

DIRECTORIES: paths in multi_FDDHpK_export.scr are currently (change as you wish, and move files) set to:

./bin			built binaries
./data			.in, .ctr, .chr, .data files and the PDB files
.			program running and pK output files

ENVIRONMENT VARIABLES: there are several parameters set by these in multi_FDDHpK_export.scr, including:

PROT_DIEL = 10
TARGET_VAL = 1.0 (VdW tolerance for sidechain repacking)

I will include more information here, hopefully very soon.

jim.warwicker@manchester.ac.uk


