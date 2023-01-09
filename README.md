# Objective

Solution to [Backend Exercise](Backend_Exercise.pdf)

## Usage

#### Prerequisites

- [`docker`](https://www.python.org/)
- [`docker-compose`](https://docs.docker.com/compose/install/)

#### Running

``` shell
DEPTH=<DEPTH> URL=<URL> docker-compose up -d
docker-compose logs -f
```

## Outputs

All pages downloaded reside in local directory called `<URL_BASE_NAME>`.  
For example: `news.ycombinator.com/`  
  
`output.tsv` file resides in `<URL_BASE_NAME>` directory  
columns: `url, depth, ratio`
