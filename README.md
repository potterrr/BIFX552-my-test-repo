# BIFX552
Bioinformatics Applications I 
## Key Discovery ##
### Using cigWin ##

When you down load files to your hard drive (e.g. in 
Swcarpentry, on the setup lesson, we download a zip file called 
data-shell.zip.)  data-shell.zip gets unpacked into a directory on the 
C: drive.  Unfortunately, Unix does not have drive letters.  That means there is no
way to get files from C://Users/Richard/Downloads/data-shell.zip to home directory of Unix.  **Except with the use of the command*mount*.  Mkdir c; mount c: /c; creates a directory c and then uses c for the c: drive.
[swcarpentry
<http://swcarpentry.github.io/shell-novice/>]

### BIFX552 Class Assignment 9/26/2019

Create one line of code that will create a specified directory structure in Unix/Ubuntu/Linux/OS

      mkdir -p HipAC/data/seqs/{fastq,bams,bams_sorted/indexed}

Now create a line of code to create files (nonexistant) into fastq directory that was just created.  The files will be named HipACs{A,B,C,D}_R{1,2}.fastq.  The command 'touch' can be used.

      touch HipAC/data/seqs/fastq/HipACs{A,B,C,D}_R{1,2}.fastq
