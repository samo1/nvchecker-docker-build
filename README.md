# nvchecker

New version checker for software releases

https://github.com/lilydjwg/nvchecker

## How to run:

* create a data directory
* create configuration file (e.g. source.ini) inside the data directory
* mount the data directory as a volume in `/home/nvchecker/data`
* run nvchecker:

```
docker run --rm -e "NVCHECKER_GITHUB_TOKEN=..." -v "$(pwd)/data:/home/nvchecker/data" samo64/nvchecker:1.4.4 nvchecker source.ini
```
