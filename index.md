## Schedule

* 10:00 - Welcome and Introduction
* 10:20 - Hacking
* 12:15 - Catch up before Lunch
* 13:15 - Hacking
* 15:45 - Wrap up
* 16:00 - End of session

## Some self-evident truths

(once you've worked in research for a while)

* Reproducibility counts
* Reproducibility doesn't happen by itself
* Open science and reproducibility go hand in hand
* You'll thank yourself later
* Technology is driving change and providing opportunities

## Organisations that care

* [Better Scientific Software][bssw]
* [The Molecular Sciences Software Institute][MolSSI]
* [Reproducibilitea]
* [Reprohack]
* [ROpenSci]
* [Society of Research Software Engineering][RSE]
* [Software Carpentry]
* [Software Sustainability Institute][ssi]
* [The Alan Turing Institute][alan-turing] and [The Turing Way]
* [The Journal of Open Source Software][joss]

[bssw]: https://bssw.io/
[MolSSI]: https://molssi.org/
[reproducibilitea]: https://reproducibilitea.org/
[reprohack]: https://reprohack.github.io/reprohack-hq/
[ropensci]: https://ropensci.org/
[RSE]: https://society-rse.org/
[software Carpentry]: https://software-carpentry.org/
[ssi]: https://www.software.ac.uk/about/manifesto
[alan-turing]: https://www.turing.ac.uk/
[the turing way]: https://the-turing-way.netlify.app/welcome
[joss]: https://joss.theoj.org/

## Defining our terms

![](https://the-turing-way.netlify.app/_images/ReproducibleMatrix.jpg)

Taken from <https://the-turing-way.netlify.app/reproducible-research/overview/overview-definitions.html>

Reproducibility is just the beginning, but it underpins the goal of
generalisable findings within a domain.

## An overview of technologies

![A diagram showing different aspects of reproducibility](https://nbis-reproducible-research.readthedocs.io/en/latest/images/tutorials_overview.png)

Taken from <https://nbis-reproducible-research.readthedocs.io/en/latest/tutorial_intro/>

## About you

* [Survey results]
* [Projects](https://github.com/ImperialCollegeLondon/rse-chemistry-hackathon/issues)

[Survey results]: https://forms.office.com/Pages/AnalysisPage.aspx?id=B3WJK4zudUWDC0-CZ8PTB5Fu0TPn6jVEtbP45q-8NH1UNFIwWjhVUFVXVzRMSlc1MzEzMFRGQjFTTS4u&AnalyzerToken=DxRTYyQcYzfokXzekAp4YCCviITDlgx0

## Resources

* [The Turing Way] is a great and very comprehensive initial resource for
  dealing with all aspects of reproducibility.
* See our [Python project template] for a quick start on new projects with
  best practice for reproducibility baked in.
* Our Graduate School Course on [Essential Software Engineering for
  Researchers][softeng] gives an introduction to several reproducibility topics
  including writing tests, managing environments and how to structure code.

[The Turing Way]: https://the-turing-way.netlify.app/reproducible-research/renv/renv-containers.html
[Python project template]: https://github.com/ImperialCollegeLondon/pytest_template_application


### Git

* The Graduate School course developed by the Imperial RSE team. Good for the
  basics before moving onto look at use of GitHub for publishing your code and
  facilitating team
  work. <https://imperialcollegelondon.github.io/grad_school_git_course/>
* <https://learngitbranching.js.org> provides a fun and interactive set of
  challenges for learning advanced features of Git to support working flexibly.
* A variety of courses pitched at different levels are available on LinkedIn
  Learning <https://www.linkedin.com/learning/topics/git>
* The relevant section of [The Turing Way][turing-git].
* An enormous amount of material exists, see [Awesome Git][] for an overview.

[turing-git]: https://the-turing-way.netlify.app/reproducible-research/vcs.html
[Awesome Git]: https://github.com/dictcp/awesome-git

### Environment Management

This is tricky one to cover in details as doing it correctly tends to vary on a
language-by-language basis. Conda is the recommended approach here due to its
flexibility in covering multiple languages as well as virtual environments.

* If you're not used to using virtual environments with Conda [this towards data
  science article][conda-env] does a good job of explaining their value. It's
  also a good initial introduction to using `environment.yml` files as the most
  robust way to manage your environments. This is Python focused but all its
  insights generalise.
* The relevant section of [The Turing Way][turing-conda]

[conda-env]: https://towardsdatascience.com/getting-started-with-python-environments-using-conda-32e9f2779307
[turing-conda]: https://the-turing-way.netlify.app/reproducible-research/renv/renv-package.html

### Containers

* [Reproducible Computational Environments Using Containers][dockerXsingularity]
  provides a good introductory guide to both Docker and Singularity with
  comparisons of both. The course was developed with researchers in mind and
  includes content on using containers in research workflows.
* [Ten simple rules for writing Dockerfiles for reproducible data
  science][rules] gives a very valuable set of pointers for using Docker in the
  context of data analysis. A must read for creating portable analyses.
* Once you've gotten the hang of Docker basics these [best practice
  tips][docker-best] will help you write clean and efficient Dockerfiles.
* A variety of courses for Docker are available on LinkedIn
  Learning. <https://www.linkedin.com/learning/search?keywords=docker>
* The relevant section of [The Turing Way][turing-containers]

[dockerXsingularity]: https://epcced.github.io/2020-12-08-Containers-Online/
[docker-best]: https://docs.docker.com/develop/develop-images/dockerfile_best-practices/
[rules]: https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1008316
[turing-containers]: https://the-turing-way.netlify.app/reproducible-research/renv/renv-containers.html

### Jupyter Notebooks/R Markdown

* As it sounds [R Markdown: The Definitive Guide][rmarkdown] is a pretty
  definitive guide with some handy examples built in.
* This blog post on [RMarkdown Driven Development][rdd] is a very interesting
  take on how to go from rough and ready data exploration to a polished document
  that cleanly tells a consistent narrative. Very relevant to Jupyter Notebooks
  as well.
* Jupyter Notebooks are extremely popular and fairly painless to start
  using. Checkout the [quick start guide][jupyter] to get up and running.
* Once you have some Notebooks take the next step to make them usable online by
  anybody with a single click via [binder][BinderHub].

[rmarkdown]: https://bookdown.org/yihui/rmarkdown/
[rdd]: https://emilyriederer.netlify.app/post/rmarkdown-driven-development/
[jupyter]: https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/index.html
[BinderHub]: https://binderhub.readthedocs.io/en/latest/

### Workflow Management

* For basic problems `make` can be a good tool if you're already familiar with
  it. Software carpentry have a [good lesson][make] on this.
* Snakemake has an ok set of [tutorials][snakemake] for getting started, though
  you'll appreciate them best with a knowledge of bioinformatics. If you're
  working on Windows I'd probably ignore the advice to use `vagrant` and use the
  `Windows Subsystem for Linux` instead.
* Nextflow should only be considered if you aren't familiar with Python. I
  struggled to find a tutorial that looked like it would work easily. Try the
  [documentation][nextflow] for an introduction and breakdown of a simple
  example.
* If you're interested in something with a user friendly graphical interface you
  could look at [Galaxy]. This takes a very different approach based on having a
  permanent server available to run workflows.

[make]: https://swcarpentry.github.io/make-novice/
[snakemake]: https://snakemake.readthedocs.io/en/stable/tutorial/setup.html#setup-a-linux-vm-with-vagrant-under-windows
[nextflow]: https://www.nextflow.io/docs/latest/getstarted.html
[Galaxy]: https://galaxyproject.github.io/

### Testing and Continuous Integration

* We cover testing in of research software in detail in our Graduate School
  course [Essential Software Engineering for Researchers][softeng]
* The Turing Way has a good section on [strategies for testing scientific
  codes][turing-testing].
* If you're going to have tests its good practice to make sure that they are run
  as part of your code hosting with continuous integration. We have an
  [experimental guide][ci] under development on this topic.

[turing-testing]: https://the-turing-way.netlify.app/reproducible-research/testing.html
[softeng]: https://imperialcollegelondon.github.io/grad_school_software_engineering_course/
[ci]: https://imperialcollegelondon.github.io/ci-best-practice/
