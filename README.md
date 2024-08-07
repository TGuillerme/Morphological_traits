# Disparity workshop - Erlangen 9th of August 2024

All the content of this course is in this [gitbook](file:///home/tguillerme/University/Teaching/Morphological_traits/gitbook/_book/index.html) if you just want to follow along online!

Alternatively, to follow this workshop and copy/paste/modify the code, the easiest is to download this whole repository (including the `example/` folder) and just follow each session in the `gitbook/` folder.

Optional: to compile the gitbook for yourself run the following:

```{r}
bookdown::render_book("gitbook/index.Rmd", "bookdown::gitbook")
```


## Schedule

| From  | To    | Details                           |
|-------|-------|-----------------------------------|
| 9:30  | 10:00 | Intro with a coffee               |
| 10:00 | 11:30 | Part 1: from traits to traitspaces |
| 11:30 | 12:00 | Part 2: from traitspaces to disparity (1) |
| 12:00 | 13:00 | **Lunch**                         |
| 13:00 | 14:00 | Part 2: from traitspaces to disparity (2) |
| 14:00 | 16:00 | Part 3: from disparity to macroevolution  |

Don't worry to much if it looks packed without much coffee breaks, they are designed within in each part to refresh your brain cells and move around a bit! 

## Content

Here's a run down of what we are going to cover:

#### Intro:

How this is going to work

[Script and notes here](/gitbook/index.Rmd)

#### Part 1:

[Script and notes here](/gitbook/01_traispaces.Rmd)

Theory:

- morphological traits
- ordination: PCA and PCO (incl. distance matrices). 

Skills:

- reading trait data into R.
- ordinating data into R.

#### Part 2:

[Script and notes here](/gitbook/02_disparity.Rmd)


Theory:

- what is disparity?
- the multidimensional nightmare.
- reducing dimensionality
- mechanisms, processes and patterns in biology

Skills:

- an intro to the dispRity package
- measuring disparity
- reducing dimensionality
- choosing and testing disparity metrics.

#### Part 3:

[Script and notes here](/gitbook/03_macroevolution.Rmd)


Theory:

- testing hypotheses with disparity
- testing hypotheses through time
- simple disparity models
- phylogenetic comparative methods and disparity? [teaser for the next day]
- disparity of disparity analyses

Skills:

- comparing disparity between groups
- comparing disparity through time
- disparity-through-time (dtt) analyses
- disparity study design
