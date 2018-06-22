PopPoly, version 1, Ehsan Motazedi (ehsan.motazedi@gmail.com), last modified: June 13 2018

Introduction
============

**PopPoly** \(executable *main.py*\) is a tool for haplotype estimation in polyploid F1 populations. PopPoly uses all of the population reads to estimate the maximum likelihood parental haplotypes, from which offspring haplotypes are selected using the MEC criterion.

The algorithm is based on a Bayesian framework to choose the most likely parental haplotypes using sequence reads, and applies Mendelian inheritance rules, assuming no recombination between the SNPs, to weight each candidate phasing for the parents and to later choose the offspring phasings from the parental haplotypes. It can also re-assign the dosages for all or missing SNPs using the Mendelian rules and sequence reads.

PopPoly is written in *Python* and is compatible with both Python 2 and Python 3.

Input parameters:
=====================

For the input parameters, see the help of the software:

./main.py --help, -h

***Example:***


./main.py bamfile vcffile output_dirname --kappa 0.85 -a 0.8 --rho 0.2 --impute


Download:
=====================
The software is available at gitlab, Wageningen UR:

git clone git@git.wageningenur.nl:motaz001/PopPoly.git —recursive

Copyright and License:
=====================
Copyright (c) 2017, Ehsan Motazedi, Wageningen UR.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files \(the "Software"\), to deal in the Software without restriction, including without limitation the rights to use, copy, share and modify the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. This permission is only valid for academic and personal use, i.e. not for commercial purposes.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

