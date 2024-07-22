## bookdown page

https://bookdown.org/yihui/rmarkdown/xaringan.html

## Slide animations

```{r}
spr <- "- Species, resources: $N_j$, $R_i$\n- Species effect on resources: $e_{ji}$"
s <- "- .red[Resource stress]: $\\red{\\omega_i}$"
f_s <- "- .green[Facilitation by resources]: $\\green{e_{fi}}$"
tp <- "- .red[Non-resource stress]: $\\red{T}$"
f_tp <- "- .green[Facilitation by non resource stress]: $\\green{f(T, F)}$"
ti <- c(
  spr,
  paste(spr, s, sep = "\n"),
  paste(spr, s, f_s, sep = "\n"),
  paste(spr, s, f_s, tp, sep = "\n"),
  paste(spr, s, f_s, tp, f_tp, sep = "\n")
)

out <- vector("character", length = 5)
for (p in seq(1, 5)) {
  out[p] <- paste0("\n\n---\n# Modelling stress and facilitation\n.pull-left[\n.left[\n```{r niche-stress-fac", p,", message=FALSE, warning=FALSE, results='asis'}\nknitr::include_graphics('images/sp_stress_facilitation_abiotic_stress_fac", p ,".png')\n```\n]]\n.pull-right[.middle[\n", ti[p], "\n]]\n")
}
```

<!--- knit those table chunk statements -->
`r paste(knitr::knit(text = out), collapse = '\n')`


## targets template

https://github.com/wlandau/targets-tutorial/tree/main/docs

## xaringan template

https://slides.yihui.org/xaringan/#1