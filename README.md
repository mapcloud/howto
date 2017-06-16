# how to install the R-kernel and the orientdb package

# Solving installation-of-package-devtools-had-non-zero-exit-status- ...

sudo apt-get install libssl-dev  # need it to install both  'httr' and 'git2r'
sudo apt-get -y install libcurl4-gnutls-dev libxml2-dev    # need for 'httr'


install.packages(c('httr', 'git2r', 'repr', 'IRdisplay', 'evaluate', 'crayon', 'pbdZMQ', 'devtools', 'uuid', 'digest'))

install.packages('devtools', repos='http://cran.rstudio.com/')
