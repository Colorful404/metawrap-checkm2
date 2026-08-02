# metawrap-checkm2
Refactor bin_refinement module to use checkm2, achieving ~50% faster analysis.

First, install micromamba. Then, create a dedicated Conda environment named checkm2 at /opt/checkm2 that contains only the CheckM2 program (the database is not included). 

This script also uses tsv-utils from https://github.com/jameslz/tsv-utils to simplify the process. This program needed to be place at the $PATH.

Checkm2 expects its database at /db/uniref100.KO.1.dmnd. We highly recommend using a container (Apptainer or Docker) to bind-mount the database to that path, rather than placing the actual file there permanently.
