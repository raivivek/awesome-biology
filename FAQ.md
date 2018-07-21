**Q. Is my BAM file sorted?**
A. Run `samtools view -H <file> | grep SO:`. If sorted, should indicate the sort order
   otherwise say `unsorted`. Further, the bam index files generated from the
   unsorted files are of smaller size (hence look fishy).


**Q. Is my data paired-end or single-end sequenced?**
A. Run `samtools flagstat <file>`; should indicate the number of reads in
   paired-end mode along with total number of reads.

Q. What are the blacklist regions across species?
A. See here: https://sites.google.com/site/anshulkundaje/projects/blacklists


Q.
