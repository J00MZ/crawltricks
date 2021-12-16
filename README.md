# Objective

Solution to [Backend Exercise](Backend_Exercise.pdf)

## Usage

### Option 1 - CLI

#### Prerequisites

- [Python](https://www.python.org/) 3.8 (with pip) or greater
- pip packages installed 
- A Redis server accessible with DNS name `redis`

#### Commands

``` shell
cd crawler
pip install -r requirements.txt
./main.py -d <DEPTH> -u <URL>
```

### Option 2 - Docker

#### Prerequisites

- [`docker`](https://www.python.org/)
- [`docker-compose`](https://docs.docker.com/compose/install/)

#### Commands

``` shell
DEPTH=<DEPTH> URL=<URL> docker-compose up -d
docker-compose logs -f
```

## Outputs

All pages downloaded reside in local directory called `<URL_BASE_NAME>`.  
For example: `news.ycombinator.com/`  
  
`output.tsv` file resides in `<URL_BASE_NAME>` directory  
columns: `url, depth, ratio`
