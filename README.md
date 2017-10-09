# ncbi-utils
utils to download, manipulate NCBI data

1. genome-download

command line interface:
    
    $ genome-download
    Usage:
       genome-download  <genome_list> <type:fna|gff|faa> <db>
       Example: genome-download  gcf.txt fna GCF
       VERSION: 0.0.1

The gcf.txt can be parsed from NCBI assembly report file:
    
     grep -P -v  ^"#" assembly_summary_refseq.txt | cut -f20  | grep -w -v  "na"  >gcf.txt
