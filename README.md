# metawrap-checkm2
Refactor bin_refinement module to use checkm2, achieving ~50% faster analysis. \n
It uses tsv-utils from https://github.com/jameslz/tsv-utils to simplify the process.
The checkm2 db must be /db/uniref100.KO.1.dmnd, it is highly recommended to use a container like apptainer or docker so you can bind the db to this path instead put the actual file right here.
