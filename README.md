# ncbi-utils
utils to download, manipulate NCBI data

1 genome-download

dependencies:
    
    # cpanm Cwd
    # wget https://github.com/brentp/gargs/releases/download/v0.3.8/gargs_linux -o  /usr/bin/gargs
   
command line interface:
    
    $ genome-download
    Usage:
       genome-download  <genome_list> <type:fna|gff|faa> <db>
       Example: genome-download  gcf.txt fna GCF
       VERSION: 0.0.1

The gcf.txt can be parsed from NCBI assembly report file:
    
     grep -P -v  ^"#" assembly_summary_refseq.txt | cut -f20  | grep -w -v  "na"  >gcf.txt
