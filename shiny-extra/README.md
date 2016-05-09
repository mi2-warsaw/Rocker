Plik `Dockerfile` oparty jest na kopii firmy rstudio https://hub.docker.com/r/rocker/shiny/~/dockerfile/ .

Po pobraniu repozytorium należy zbudować Dockera z shiny-server'em z rozszerzona listą pakietów poleceniem

`docker build -t shiny-extra:latest .` w folderze `shiny-extra`

uruchomić Docker z shiny-serverm'em i rozszerzoną listą pakietów można poleceniem

```{R}
docker run --rm -p 3838:3838 \
    -v /srv/shiny-server/:/srv/shiny-server/ \
    shiny-extra:latest
```