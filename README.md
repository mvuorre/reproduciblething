# reproduciblething

A template for reproducible manuscripts with R

reproduciblething aims to set in place the following tools for setting up a practically reproducible manuscripts:

- renv: Ensure a reproducible R package environment
- environment variables
  - To handle e.g. expensive computations do not prevent evaluation of reproducibility
- Reasonable but non-restrictive template(s) for data analyses and outputs
  - <https://github.com/wjschne/apaquarto>

## Requirements

- Everything required to run `renv::restore()` in R on a computer
- (Optional) [RStudio](https://posit.co/downloads/)
- (Optional) [Quarto](https://quarto.org/)
- (Optional) [GNU Make](https://www.gnu.org/software/make/)
  - Included in Linux & MacOS but not Windows

## What's in the template?

I assume that the end product you want is an academic manuscript or something similar. This template then provides

- renv
- Makefile
- .Renviron.example
- apaquarto template

When these are set up, `make` goes from 0 to manuscript.pdf/docx/html?

[todo]: Does this even need a new template? Well I always end up fiddling with the Makefile and loading relevant variable in source. I guess I want to make this for myself so that the author info is prefilled?

## Use

tbd

Maybe as a quarto extension with `quarto use mvuorre/reproduciblething` this has the benefit of also working with clone / download on GitHub.

## Motivation

Full reproducibility is not possible because we cannot ask others to build DIY computers that run code or power plants that produce electricity. What we can achieve is *practical reproducibility*: Assuming some common tools are already in place, clients (end-users) can build the project with minimum fuss.

One might propose that the gold-standard for achieving practical reproducibility is Docker. However, developers (initial analysts, original authors) do not know Docker and learning and using it consistently is associated with overheads that are too expensive for most developers. I (MV) feel similarly about the targets R package.

The vision for practical reproducibility in this template is then based on the "Do not let perfect be the enemy of the good" mantra. 
