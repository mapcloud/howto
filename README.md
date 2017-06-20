# how to install the R-kernel and the orientdb package ubuntu 16.04

follow this blog [Jupyter And R Markdown: Notebooks With R](https://www.datacamp.com/community/blog/jupyter-notebook-r#alternatives) but first look make sure you have installed the following packages to avoid the devtools installation error.


# Solving installation-of-package-devtools-had-non-zero-exit-status- ...

    sudo apt-get install libssl-dev  # need it to install both  'httr' and 'git2r'
    sudo apt-get -y install libcurl4-gnutls-dev libxml2-dev    # need for 'httr'

    install.packages(c('httr', 'git2r', 'repr', 'IRdisplay', 'evaluate', 'crayon', 'pbdZMQ', 'devtools', 'uuid', 'digest'))

    # install.packages('devtools', repos='http://cran.rstudio.com/')

solutions from [installing-devtools-fails-beacuse-of-dependency-but-dependency-is-not-available](https://stackoverflow.com/questions/35063883/installing-devtools-fails-beacuse-of-dependency-but-dependency-is-not-available)

and [installation-of-package-devtools-had-non-zero-exit-status-in-a-powerpc](https://stackoverflow.com/questions/31114991/installation-of-package-devtools-had-non-zero-exit-status-in-a-powerpc), however no need to be root.
