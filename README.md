# reproduciblething

A template for reproducible manuscripts with R

reproduciblething aims to set in place the following tools for setting up a practically reproducible manuscripts:

- renv: Ensure a reproducible R package environment
- environment variables
  - To handle e.g. expensive computations do not prevent evaluation of reproducibility
- Reasonable but non-restrictive template(s) for data analyses and outputs
  - Would love Quarto but I guess papaja?

## Requirements

- Everything required to run `renv::restore()` in R on a computer
- (Optional) [RStudio](https://posit.co/downloads/)
- (Optional) [Quarto](https://quarto.org/)
- (Optional) [GNU Make](https://www.gnu.org/software/make/)
  - Included in Linux & MacOS but not Windows

## Use

tbd

Maybe as a quarto extension with `quarto use mvuorre/reproduciblething` this has the benefit of also working with clone / download on GitHub.

## Motivation

Full reproducibility is not possible because we cannot ask others to build DIY computers that run code or power plants that produce electricity. What we can achieve is *practical reproducibility*: Assuming some common tools are already in place, clients (end-users) can build the project with minimum fuss.

One might propose that the gold-standard for achieving practical reproducibility is Docker. However, developers (initial analysts, original authors) do not know Docker and learning and using it consistently is associated with overheads that are too expensive for most developers. I (MV) feel similarly about the targets R package.

The vision for practical reproducibility in this template is then based on the "Do not let perfect be the enemy of the good" mantra. 
