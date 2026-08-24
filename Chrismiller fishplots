#depending on the origins of the clones (original new clones or subclones) you should state its origin (0,1,2,3 etc).Certo — se vuoi **una sezione README per il tuo GitHub**, nello stesso stile ma riferita al fatto che utilizzi/integri il package `fishplot`, puoi scriverla così:

## Fishplot

An R package for visualizing changes in the subclonal architecture of tumors.

In this project, `fishplot` is used to visualize the dynamics of tumor subclones across different timepoints, providing an intuitive representation of clonal evolution and population changes.

### Installation

Install the package directly from GitHub using `devtools`:

```r
# Install devtools if you don't have it already
install.packages("devtools")

library(devtools)
install_github("chrisamiller/fishplot")
```

### Usage

The package requires:

* a set of timepoints;
* a matrix containing the fraction of each clone at each timepoint;
* a vector defining the parent of each clone.

Example:

```r
library(fishplot)

# Define the timepoints
timepoints <- c(0, 30, 75, 150)

# Fraction of each population at each timepoint
frac.table <- matrix(
  c(100, 45, 0, 0,
    2,   0, 0, 0,
    2,   0, 2, 1,
    98,  0, 95, 40),
  ncol = length(timepoints)
)

# Define the parent of each clone
# 0 indicates that the clone has no parent
parents <- c(0, 1, 1, 3)

# Create the fishplot object
fish <- createFishObject(
  frac.table,
  parents,
  timepoints = timepoints
)

# Calculate the layout
fish <- layoutClones(fish)

# Generate the plot
fishPlot(
  fish,
  shape = "spline",
  title.btm = "Sample1",
  cex.title = 0.5,
  vlines = c(0, 150),
  vlab = c("day 0", "day 150")
)

### Reference

This project uses the [`fishplot`](https://github.com/chrisamiller/fishplot) R package developed by Chris Miller for the visualization of tumor subclonal architecture.
c
