# R Packages for Jimmy Briggs ([`jimbrig`](https://github.com/jimbrig))

> [!NOTE]
> This repository hosts the [`packages.json`](packages.json) configuration file used to build my [R Universe](https://jimbrig.r-universe.dev/).

- **Live Site:** <https://jimbrig.r-universe.dev/>
- **GitHub Repository:** <https://github.com/r-universe/jimbrig>

## Configuration

All configuration is housed in the [`packages.json`](packages.json):

<details><summary>View Code</summary><p>

```json
[
  {
    "package": "jimstools",
    "url": "https://github.com/jimbrig/jimstools"
  },
  {
    "package": "lossrx",
    "url": "https://github.com/jimbrig/lossrx"
  },
  {
    "package": "losdevtapp",
    "url": "https://github.com/jimbrig/lossdevtapp"
  },
  {
    "package": "configR",
    "url": "https://github.com/jimbrig/configR"
  },
  {
    "package": "templateeR",
    "url": "https://github.com/jimbrig/templateeR"
  },
  {
    "package": "browsr",
    "url": "https://github.com/jimbrig/browsr"
  },
  {
    "package": "buildtools",
    "url": "https://github.com/jimbrig/buildtools"
  },
  {
    "package": "rtraining",
    "url": "https://github.com/jimbrig/rtraining"
  }
]
```

</p></details>

 ## Adding New Packages

 Make a new pull-request to append an entry to the [`packages.json`](packages.json) file, i.e.:

 ```json
{
  "package": "<packageName>",
  "url": "https://github.com/jimbrig/<packageName>"
}
```

## Installing Packages

To install a package from my universe, utilize the following syntax:

```R
install.packages("<packageName>", repos = "https://jimbrig.r-universe.dev")
```

alternatively, configure the `repos` option:

```R
options(
    repos = c(
        jimbrig = "https://jimbrig.r-universe.dev",
        CRAN = "https://cloud.r-project.org"
    )
)
install.packages("<packageName>")
```


