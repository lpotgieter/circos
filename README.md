# Workflow

runs with promer or nucmer from [https://mummer4.github.io/manual/manual.html](https://mummer4.github.io/manual/manual.html) to obtain links/alignment file. not really necessary. but often users want this
in its most basic form

`promer [options] <reference> <query>`

`show-coords promer.delta > promer.coords `

change input files in [coords2links.py](https://github.com/lpotgieter/circos/blob/main/coords2links.py)

produce karyotype files from reference fasta with [fasta2kar.sh](https://github.com/lpotgieter/circos/blob/main/fasta2kar.sh)

optionally, add a column in the karyotype file that has the colour you want each block to have. nice to have two different colours if you want to show pairwise genome alignment

the [circos config](https://github.com/lpotgieter/circos/blob/main/circos_config.config) is the most challenging to produce. this worked on [circos-0.69-9](https://circos.ca) 


to run circos
`circos -conf circos_conf.conf` 
