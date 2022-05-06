# Supplementary material for *A genetic algorithm for fair land allocation*

This repository holds the source code, instances, instance generator and detailed result tables for the following paper:

> **A genetic algorithm for fair land allocation**<br>
> Alex Gliesch, Marcus Ritt and Mayron C.O. Moreira (2017) <br>
> Genetic and Evolutionary Computation Conference (GECCO), pp. 793-800 <br>
> https://doi.org/10.1145/3071178.3071313

**Bibtex**

```bibtex
@inproceedings{Gliesch.etal/2017,
  title        = {A genetic algorithm for fair land allocation},
  author       = {Gliesch, Alex and Ritt, Marcus and Moreira, Mayron CO},
  booktitle    = {Genetic and Evolutionary Computation Conference},
  pages        = {793--800},
  year         = {2017},
  organization = {ACM},
  doi          = {10.1145/3071178.3071313}
}
```

Please use the reference above if you use this material in your research.

## Running the code 
1. Under `src`, compile with `make release`. For logging messages and other checks, use `make debug`.
1. Run using `./proterra --in {instance} --time {timeLimit} --png {outFile}`. For more options, see `--help`.

## Generating instances
1. Under `instances/instance-generator`, run `make`.
1. Run `./generate -w {width} -h {height} --lots {numLots} --river_ct {riverPercentage} --apt {numAptitudeClasses}`.