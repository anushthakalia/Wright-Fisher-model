# The Wright Fisher Model
The aim of the study was to study the evolution of allele frequencies in a finite population. This notebook describes a very
basic model which assumes:
* Population size:    constant, N

* Structure of the genome:   one single haploid chromosome of length 1 base pair. 

* Mode of reproduction:      asexual

* Mutation process:          No mutation

* Transmission:              Asexual transmission (clonal reproduction)

Below are the figures that were generated.
## Probability distribution of alternate alleles
Number of populations (samples drawn) = 1000<br>
__Population size = 50__<br>
<img src='images/1.png'><br>
__Population size = 100__ <br>
<img src='images/2.png'><br>
## Mean frequency of alternate allele across 100 generations 
The graph below displays the mean allelic frequencies for 100 generations (plus the initial population).<br>
<img src='images/3.png'><br>
## Population frequency of 1 allele across 30 generations
Number of populations = 10<br>Population size of one generation = 100<br>Intial p0 = 0.3<br>
<img src='images/4.png'><br>
Number of populations = 1000<br>Population size of one generation = 100<br>Intial p0 = 0.3<br>
<img src='images/5.png'><br>
## Plots for allele frequency across 1000 populations for 30 generations
### Line Plot
<img src='images/6.png'><br>
### Density Map
<img src='images/7.png'><br>
### 3-D Histogram
<img src='images/8.png'><br>
## Effect of population size on distribution of allele frequencies
<img src='images/9.png'><br>
### Relation between expected changes in allele frequencies (variance) and population size
The allele counts of a particular generation follow
binomial distribution (for large populations poisson). The variance is given by N*p*(p-1), where N is the size of 
the population and p is frequency of alternate allele in the current population.
p equals p0 for the current population and is a constant. Hence,
the relation between population size and variance is linear.<br>
<img src='images/10.png'><br>
## Effect of initial allele frequency on distribution of allele frequencies
<img src='images/11.png'><br>
### Relation between expected changes in allele frequencies (variance) and initial allele frequency
Again if we consider the relation of Var=N*p*(p-1), we get a quadratic equation. And, in fact the data supports this theory.
Also, its simpler than any trignometric function!<br>
<img src='images/12.png'><br>
## Mutations
### Line Plot for allelic frequencies across 100 generations
Number of populations = 2000  
Number of generations = 100  
Size of each population = 10  
Mutations introduced initially = 1/10  
<img src='images/13.png'><br>
### Generation vs fixation probability
