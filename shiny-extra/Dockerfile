FROM rocker/shiny:latest 

MAINTAINER Marcin Kosiński "m.p.kosinski@gmail.com"

# install additional packages
RUN R -e "install.packages('tidyverse')"
RUN R -e "install.packages(c('shinydashboard', 'leaflet', 'ggmap', 'stringi', 'RSQLite', 'DT', 'ggvis'), repos='https://cran.rstudio.com/')"
RUN R -e "install.packages(c('knitr', 'pander', 'wordcloud'), repos='https://cran.rstudio.com/')"

CMD ["/usr/bin/shiny-server.sh"]
