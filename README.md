## UndergraduateGenomicsTraining

Here are some tasks we are going to work through together in todays session. Each one uses a combination of commands we have covered so far. 

## Task 1 - Setting up a project directory

Here we want to set up a directory ready for a project. 
1. start in the home directory 
2. make a new directory (with a command that won't override a file that already exists) called `NewProject`
3. within that directory make three new ones - `Data`, `Analysis`, `Output`
4. count the number of `fastq` files in the directory `/hb/groups/kelley_training/rawdata`
5. make a sample list of these `fastq` files
6. move the sample list to our `Data` folder
7. check that the file looks correct after moving it by looking in it
8. check the last line(s) of the file and make sure they are complete
9. check what modules are installed on the cluster
10. see if the software `fastqc` is installed and which version(s) we can use


## Task 2 - QC our data

Here we want to run a QC on our data - is it any good? 
1. make a new directory (with a command that won't override a file that already exists) called `NewProject`
2. within that directory make three new ones - `Data`, `Analysis`, `Output`
3. move into our analysis folder
4. make a new script called `01_fastqc.sh`
5. add the necessary first line in this file
6. add the slurm details we need to tell the cluster what kind of job we are running
7. save the script
8. make a symbolic link for the fastq file `/hb/groups/kelley_training/rawdata/SST513_1_USR18001329L_HCCVGDMXX_L1_1.fq.gz`
9. make a symbolic link for the fastq file `/hb/groups/kelley_training/rawdata/SST513_1_USR18001329L_HCCVGDMXX_L1_2.fq.gz`
10. add the module load lines from the version we found before
11. add a line that makes an output directory `fastqc_output` (remember - no spaces in file or folder names!)
12. add the line to run fastqc speficying two threads, our ourput directory, and the fastq file


## Task 3 - Trim our data

Make a script to trim one set of reads `/hb/groups/kelley_training/rawdata/SST513_1_USR18001329L_HCCVGDMXX_L1_1.fq.gz` and `/hb/groups/kelley_training/rawdata/SST513_1_USR18001329L_HCCVGDMXX_L1_2.fq.gz`


## Some handy bash tips:
`cd`: This command changes the current directory.  
`ls`: This command lists the contents of a directory.  
`ls -lh`: This command lists the contents of a directory including file sizes, permissions, and extra info.  
`pwd`: This command prints the current working directory.  
`mkdir`: This command creates a new directory.  
`mkdir -p`: This command creates a new directory - but only if the directory doesn't already exist.  
`rmdir`: This command removes an empty directory.  
`cp`: This command copies a file or directory.  
`mv`: This command moves a file or directory.  
`rm`: This command removes a file or directory.  
`cat`: This command concatenates and prints files.  
`less`: This command helps us view files.  
`head`: This command prints the first few lines of a file.  
`tail`: This command prints the last few lines of a file.  
`>`: This lets us 'pipe' output from one command into a file.  
