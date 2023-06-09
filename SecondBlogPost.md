Programming Background
================

    github_document(
      toc = FALSE,
      toc_depth = 3,
      number_sections = FALSE,
      math_method = "default",
      preserve_yaml = FALSE,
      fig_width = 7,
      fig_height = 5,
      dev = "png",
      df_print = "default",
      includes = NULL,
      md_extensions = NULL,
      hard_line_breaks = TRUE,
      pandoc_args = NULL,
      html_preview = TRUE,
      keep_html = FALSE
    )

    library(rmarkdown)
    render("SecondBlogPost.Rmd",
            output_format = "markdown"
            output_dir = "C://Users/monicabeingolea/Documents/ST558/sjwilli6.github.io/sjwilli6.github.io/SecondBlogPost/_Rmd.md"
            output_options = list(md_extensions = "-markdown_in_html_blocks")
            )

## Thoughts on R

I have used a couple different software programs in my career and at
NCSU. I have used SAS, R, JMP, and Prism. I enjoy using R as my
software, because there are plenty of resources online to help with my
coding if I get stuck. I enjoy the different functions and collection of
libraries that are available with R. I have never used GitHub before, so
I am looking forward to working with GitHub and R collectively. Since I
use JMP and Prism almost every day in my work, I know the ins and outs
of these software. Sometimes with R, I find myself having to search
online in order to resolve my code which can take some time. I believe
that having previous SAS experience in undergrad and other grad classes
has helped me with learning R. Having any software experience helps
understand what we are trying to code.

## Example Rmarkdown output

    knitr::opts_chunk$set(fig.path = "../images/")

    plot(iris)
