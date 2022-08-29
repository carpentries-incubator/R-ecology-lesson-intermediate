---
title: "Lessson introduction"
teaching: 10
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions 

- How should I use this lesson?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Understand how to use this lesson as a follow-up to the Data Carpentry R for Ecology lesson
- Understand how to use this lesson as a standalone lesson for intermediate R users

::::::::::::::::::::::::::::::::::::::::::::::::

## About this lesson

This lesson was originally the final episode of the updated R for Ecology lesson, and was designed as an optional follow-up to the prior episodes. The R for Ecology lesson uses a cleaned dataset from the earlier years of the Portal rodent data, which is suitable for new R learners. This data for this lesson comes from more recent years of the Portal data, spread across 3 data files, and in an "uncleaned" form. It introduces only a handful of new `tidyverse` functions and focuses primarily on putting previously learned skills to use in real-world scenarios, combining them to build pipelines, and extending them to new use cases.

## Use as a follow-up lesson

- recommended for intermediate skill level
- may cause burnout if you try to cram it in
- best used if learners are speeding through the R Ecology lesson

## Used standalone

- probably need to do a little bit of introduction of the dataset, like first part of R Ecology ggplot lesson


```r
library(ratdat)
?complete_old
str(complete_old)
```

```{.output}
'data.frame':	16878 obs. of  13 variables:
 $ record_id      : int  1 2 3 4 5 6 7 8 9 10 ...
 $ month          : int  7 7 7 7 7 7 7 7 7 7 ...
 $ day            : int  16 16 16 16 16 16 16 16 16 16 ...
 $ year           : int  1977 1977 1977 1977 1977 1977 1977 1977 1977 1977 ...
 $ plot_id        : int  2 3 2 7 3 1 2 1 1 6 ...
 $ species_id     : chr  "NL" "NL" "DM" "DM" ...
 $ sex            : chr  "M" "M" "F" "M" ...
 $ hindfoot_length: int  32 33 37 36 35 14 NA 37 34 20 ...
 $ weight         : int  NA NA NA NA NA NA NA NA NA NA ...
 $ genus          : chr  "Neotoma" "Neotoma" "Dipodomys" "Dipodomys" ...
 $ species        : chr  "albigula" "albigula" "merriami" "merriami" ...
 $ taxa           : chr  "Rodent" "Rodent" "Rodent" "Rodent" ...
 $ plot_type      : chr  "Control" "Long-term Krat Exclosure" "Control" "Rodent Exclosure" ...
```

- everything else in the lesson is standalone, but it assumes learners are familiar with working with dataframes, the basics of `ggplot2`, `filter()`, `select()`, `group_by()`, `mutate()`, and `summarize()`
