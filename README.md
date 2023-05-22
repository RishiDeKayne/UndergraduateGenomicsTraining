## UndergraduateGenomicsTraining

Here are some tasks we are going to work through together in todays session. Each one uses a combination of commands we have covered so far. 

## Task 1 - Setting up a project directory

Here we want to set up a directory ready for a project. 
1. start in the home directory 
2. make a new directory (with a command that won't override a file that already exists) called `NewProject`
3. within that directory make three new ones - `Data`, `Analysis`, `Output`
4. count the number of `fastq` files in the directory `xxxxx`
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
8. make a symbolic link for the fastq file `xxxxx`
9. add the module load lines from the version we found before
10. add a line that makes an output directory `fastqc_output` (remember - no spaces in file or folder names!)
11. add the line to run fastqc speficying two threads, our ourput directory, and the fastq file


## Task 3 - Trim our data

Here we want to trim our data using Trimmomatic
