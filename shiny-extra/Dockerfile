FROM rocker/shiny:latest 

MAINTAINER Marcin Kosiński "m.p.kosinski@gmail.com"

# install additional packages
RUN R -e "install.packages(c('shinydashboard', 'leaflet', 'dplyr', 'ggmap', 'stringi', 'RSQLite', 'DT', 'ggplot2', 'ggvis', 'jsonlite', 'knitr', 'pander', 'readr', 'wordcloud', 'tibble'), repos='https://cran.rstudio.com/')"

CMD ["/usr/bin/shiny-server.sh"]
