FROM rocker/shiny:latest 

MAINTAINER Marcin Kosiński "m.p.kosinski@gmail.com"

# install additional packages
RUN R -e "install.packages(c('shinydashboard', 'leaflet', 'dplyr', 'ggmap', 'stringi', 'RSQLite', 'DT'), repos='https://cran.rstudio.com/')"

CMD ["/usr/bin/shiny-server.sh"]
