---
title: "Lesson 17: Wrapping up and looking ahead"
output: 
  html_document:
    keep_md: yes 
    toc: true
---



<br>

## Today is our last class! 
Thank you for joining us this semester and for your patience and understanding as we have been navigating the online format. It has been great to have you all in the course.

<br>

## Course evaluations
#### Please complete the course evaluations when they become available at the end of the semester
Unfortunately, we will not be able to get our course evaluations until the end of the semester. Students formally enrolled (both for credit or audit) should get an email with a link to the evaluation at that time, and I would really appreciate it if you can take a few minutes to answer the questions.

This is the second time I have offered this course, and it is still under very active development. I'm currently in the process of turning it into a permanent course (NTRES 6100), so I would really value everybody's feedback on how we can improve it and make it as useful as possible.

Please share your candid thoughts and suggestions in the evaluation. Remember that all comments are completely anonymous and I only get to see it after S/U decisions have been submitted. 

If anyone has feedback or suggestions they would like to share right away, we would be happy to hear your thoughts! You can either private message, email, or post in the `feedback` channel on Slack. Remember you can post anonymously by prefacing your message with `/anon ` (e.g. `/anon Here is my message).

<br>

## Agenda for today's class

* Student presentations - we're looking forward to hearing from you!
* If there is time: A quick review of some good practices
* Where to learn more and connect with the R user community
* Important take-home messages

<br>
<br>

## Good practices

<br>
 
### 1. Keep your raw data raw
Resist the temptation to manually edit or reformat your original file because if your documentation of the changes is imperfect, you may lose important information.
Clean up the data in R. Your R code, along with appropriate documentation will be a record of the changes. The code can be modified and rerun, using the raw data file as input, if needed.

<br>

### 2. Make sure all your processing steps are included in your scripts and test that your code can run in a new environment
Make sure that your code does not rely on objects or functions defined outside of your script. If that is the case, it can't readily be run by yourself or someone else in the future. 

Make sure to frequently re-start R as you're working, as elaborated on by Jenny Bryan [here](https://www.tidyverse.org/blog/2017/12/workflow-vs-script/).

Also, if you haven't already, follow the [instructions from r4ds](https://r4ds.had.co.nz/workflow-projects.html#what-is-real) on how ensure that RStudio does not restore your workspace between sessions, so you start with a clean environment every time. Make sure this option is selected under your RStudio preferences:

<img src="assets/rstudio-workspace.png" width="50%" />
   
<br>
<br>


Slides from [Deep thoughts](https://www.slideshare.net/jenniferbryan5811/cm002-deep-thoughts) by Jenny Bryan:

![](assets/small-mistake.png)

<br>
<br>


![](assets/redo-analysis.png)

<br>

### 3. Organizing your work into R projects within RStudio makes life easier
Organizing your work into RStudio projects avoids issues with absolute file paths and makes it easier to keep track of the code used to generate plots and reports, share your code with others, and work on multiple different projects in parallel. Not convinced yet? Check out [What they forgot to teach you about R](https://rstats.wtf/project-oriented-workflow.html)

<br>

### 4. Explain and document your thought process with notes and comments
Document the big-picture structure both within files (comments) and between files (README’s). In general, comments (and Git commit messages) should explain the why not the what (which should be self-evident from well-written code). Can a collaborator or you-in-six-months quickly figure out what’s going on in your code?

<br>

### 5. Develop a consistent coding style that maximizes readability
Developing a consistent style in your coding, makes it a lot easier to read. Here is some inspiration:

* The [tidyverse style guide](https://style.tidyverse.org/)
* A more [concise overview of the style Hadley Wickham uses](http://adv-r.had.co.nz/Style.html) in his books "R for Data Science" and "Advanced R"
* There are also great tips for styling, organizing and optimizing your code in the blogpost [R Best Practices: R you writing the R way!](https://blog.quantinsti.com/r-best-practices-r-you-writing-the-r-way/?utm_campaign=News&utm_medium=Community&utm_source=DataCamp.com) by Milind Paradkar
* Many of the same principles are also summarized by JEFworks [here](https://jef.works/R-style-guide/)

<br>

### 6. "Write code for humans, write data for computers"
Very important advice from [Vince Buffalo](https://twitter.com/vsbuffalo/status/358699162679787521) 

Reshape your data into tidy format for analysis. That way, you can take advantage of the powerful set of tools available in the tidyverse and beyond instead of having to invent your own roundabout approaches, and this will both make your code more robust, concise, and readable.

Some ways to make code more human-readable include:

* Clear workflows
* Use comments
* Give objects meaningful names
* Use well-named operations, e.g. `select(data, columnname)` instead of `data[,5]`


<br>
<br>

## Resources for learning more

<br>

#### R and the tidyverse

* [R for Data Science](https://r4ds.had.co.nz/) by Garrett Grolemund and Hadley Wickham. See also answers to the exercises [here](https://jrnold.github.io/r4ds-exercise-solutions/) and other places you can find on google and a dedicated [R4DS Slack workspace](https://www.rfordatasci.com/) for community learning. [I strongly recommend working through the chapters of this book that we have not covered]
* [Advanced R](https://adv-r.hadley.nz/) by Hadley Wickham
* [swirl: learn R, in R](https://swirlstats.com/) - a platform for learning R programming and data science interactively, at your own pace, and right in the R console
* [What they forgot to teach you about R](https://rstats.wtf/) by Jenny Bryan and Jim Hester
* [Course notes for STAT545](https://stat545.com/) by Jenny Bryan
* [Practical Data Science for Stats - a PeerJ Collection](https://peerj.com/collections/50-practicaldatascistats/)
* [ggplot2: Elegant Graphics for Data Analysis](https://ggplot2-book.org/) by Hadley Wickham

<br>

Here are a few other books you might want to check out:

* [A ModernDive into R and the tidyverse](https://moderndive.com/) by Chester Ismay and Albert Y. Kim  
* [The R Cookbook](https://rc2e.com/) by James Long and Paul Teetor  
* [Introduction to Data Science: Data Analysis and Prediction Algorithms with R](https://rafalab.github.io/dsbook/) by Rafael A. Irizarry  


And for getting help, check out the [slide deck](https://resources.rstudio.com/rstudio-conf-2020/object-of-type-closure-is-not-subsettable-jenny-bryan) or [recorded talk](https://speakerdeck.com/jennybc/object-of-type-closure-is-not-subsettable?slide=12) for Jenny Bryan's talk "Object of type ‘closure’ is not subsettable" at the 2020 RStudio conference. You can also check out her [Reprex webinar](https://resources.rstudio.com/webinars/help-me-help-you-creating-reproducible-examples-jenny-bryan). 

<br>

#### RMarkdown

* [RMarkdown for Scientists](https://rmd4sci.njtierney.com/) by Nicholas Tierney
* [R Markdown: The Definitive Guide](https://bookdown.org/yihui/rmarkdown/) by Yihui Xie, J. J. Allaire, and Garrett Grolemund

<br>

#### GitHub

* [Happy Git and GitHub for the useR](https://happygitwithr.com/) by Jenny Bryan

<br>

#### Open practices in environmental data science

* Check out and follow developments at [Openscapes](https://www.openscapes.org/), an awesome organization led by Julia Stewart Lowndes aimed at empowering environmental scientists to do better science in less time through open and collaborative practices.

<br>

### More cool R applications

**Dashboards:**

Check out the [Dashboard](https://ramikrispin.github.io/coronavirus_dashboard/#summary) developed for the continually updated [Coronavirus dataset](https://github.com/RamiKrispin/coronavirus) we worked with earlier in the course. Note that you can grab all the code under `Source code` in the top right corner.

Dashboards can also be made interactive with dynamic and user-controlled displays of data through use of [Shiny](https://shiny.rstudio.com/), an R package that makes it easy to build interactive web apps straight from R.

For an example, check out [this dynamic visualization](https://uomresearchit.github.io/r-shiny-course/) of the gapminder dataset we worked with in our last class (make sure to check out the [cool video](https://www.youtube.com/watch?v=jbkSRLYSojo) with Hans Rosling) 

[Here](https://rebjoh.shinyapps.io/Gapminder-app/) is a much simpler shiny app with interactive display of the same data.

For more examples, check out the [RStudio Flexdashboard website](https://rmarkdown.rstudio.com/flexdashboard/). And check out [Mastering shiny](https://mastering-shiny.org/) by Hadley Wickham

<br>

## Connecting with the R stats community 
[Tips on how to start engaging on twitter](https://rstudio-conf-2020.github.io/r-for-excel/collaborating.html#r-communities) from R for Excel Users by Julia Lowndes and Allison Horst 

and

[Finding the YOU in the R community](https://github.com/jthomasmock/presentations/blob/master/r-community2.pdf) by Thomas Mock

<br>

## Take-home messages

> From the [Ocean Health Index Data Science Training](http://ohi-science.org/data-science-training/champion.html#three-messages):

### Three messages

If there are 3 things to communicate to others after this workshop, I think they would be: 

<br>

**1. Data science is a discipline that can improve your analyses**

- There are concepts, theory, and tools for thinking about and working with data. 
- Your study system is not unique when it comes to data, and accepting this will speed up your analyses.

*This helps your science:*

- Think deliberately about data: when you distinguish data questions from research questions, you'll learn how and who to ask for help
- Save heartache: you don’t have to reinvent the wheel
- Save time: when you expect there’s a better way to do what you are doing, you'll find the solution faster. Focus on the science.

<br>

**2. Open data science tools exist**

- Data science tools that enable open science are game-changing for analysis, collaboration and communication.
- Open science is "the concept of transparency at all stages of the research process, coupled with free and open access to data, code, and papers" ([Hampton et al. 2015](http://onlinelibrary.wiley.com/doi/10.1890/ES14-00402.1/abstract)))  

*This helps your science:*

- Have confidence in your analyses from this traceable, reusable record
- Save time through automation, thinking ahead of your immediate task, reduced bookkeeping, and collaboration
- Take advantage of convenient access: working openly online is like having an extended memory

<br>

**3. Learn these tools with collaborators and community (redefined):** 

- Your most important collaborator is Future You. 
- Community should also be beyond the colleagues in your field.
- Learn from, with, and for others. 

*This helps your science:* 

- If you learn to talk about your data, you'll find solutions faster. 
- Build confidence: these skills are transferable beyond your science.
- Be empathetic and inclusive and build a network of allies 


<br>

## Discussion questions to follow up on presentations (if there is more time)

* What is the most valuable thing you have learned in this class?
* Are you planning to implement any changes your workflow or practices moving forward
* What are you excited about learning next or what existing skills do you want to improve?

