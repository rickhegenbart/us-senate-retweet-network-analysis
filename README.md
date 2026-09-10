# U.S. Senate Retweet Network Analysis

> **Master’s Psychology Research & Analytics Portfolio**
>
> This project was completed as part of my Master’s degree program in Psychology. It applies R-based social-network analysis to examine public retweet relationships among U.S. Senate accounts.
>
> [View the complete Master’s Psychology Research & Analytics Portfolio](https://github.com/users/rickhegenbart/projects/1)

## Overview

This R Markdown project analyzes public retweet relationships among U.S. Senate accounts.

The analysis collects public posts, constructs directed retweet networks, calculates graph metrics, identifies communities, and creates interactive network visualizations.

This is a nonpartisan academic analysis of public social-media interactions. It does not evaluate political positions, endorsement, or the accuracy of account content.

## Analysis Questions

* Which Senate accounts appear in the retweet network?
* How many nodes and connections are present?
* How dense is the retweet network?
* Which accounts have the highest number of direct network connections?
* What communities emerge from retweet relationships?
* How do retweet patterns appear in interactive network visualizations?

## Methods

The analysis:

* Retrieves public timeline and list data through the X/Twitter API.
* Builds retweet-edge data from account interactions.
* Creates directed network graphs with `igraph`.
* Calculates vertex count, edge count, density, and degree.
* Identifies communities with the Infomap algorithm.
* Creates interactive network visualizations with `visNetwork`.
* Displays account-level network metrics in interactive tables.

## Tools

* R
* R Markdown
* `tidyverse`
* `igraph`
* `visNetwork`
* `DT`
* `rtweet`
* `graphTweets`

## Data and Security

The project retrieves public social-media data through the X/Twitter API.

API credentials are not included in this repository. To run the analysis, configure approved credentials locally through environment variables. Do not commit API keys, tokens, `.Renviron` files, or downloaded data that cannot be redistributed.

Platform access, API requirements, available data, and package compatibility may change over time.

## Repository Contents

```text
├── README.md
└── USSenate(20260910-202654).Rmd
```

## Reproducing the Analysis

Install the required R packages:

```r
install.packages(c(
  "tidyverse", "ggplot2", "DT", "igraph",
  "rtweet", "visNetwork", "graphTweets"
))
```

Configure valid API credentials locally, then render the R Markdown file with active internet access.

## Project Status

This repository preserves the original social-network-analysis source code. A reproducible HTML report can be added after the credentials are removed and the data-retrieval workflow is updated and tested.
