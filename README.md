# mediationSoftwareReviewJEBS
replication material for "Review: mediation Package in R" in JEBS (2016)

Here's a link to the published version:
https://journals.sagepub.com/doi/full/10.3102/1076998616670371

To replicate, in `R`, set the working directory to the directory where you cloned this repo, and run
```
Sweave('mediationSoftwareReview.Rnw')
```
This step takes 4-5 minutes on my laptop. 
It will load the version of the `mediation` package that was current when the paper was written
(I don't know if it's changed substantially, but just in case it has, this should replicate the paper).

Then, complile the `.tex` file, e.g. by running (on the command line)
```
pdflatex mediationSoftwareReview.tex
bibtex mediation
pdflatex mediationSoftwareReview.tex
pdflatex mediationSoftwareReview.tex
```
