# REQ8

> Manage HTTP RESTful APIs per-project in YAML files.

## SYNOPSIS

req8 uses the terminal to allow developers to manage per-project
API requests via YAML files.

req8 supports dynamic environments and header presets with Python's natural
string templating.

Currently req8 requires python and incorporates a visual selection
picker for missing arguments.

## DEMO

![req8 demo](http://rafi.io/static/img/project/req8/demo.gif)

## USAGE

Create a `.requests.yml` file in your project directory, and run `req8`:

```sh
$ ./req8 -h
usage: req8 [-h] [-e ENVIRONMENT] [-s] [resource] [request]

positional arguments:
  resource              Key name of resource
  request               Name of request

optional arguments:
  -h, --help            show this help message and exit
  -e ENVIRONMENT, --environment ENVIRONMENT
                        Specify environment's key name
  -s, --show-headers    Show
```

## EXAMPLE USAGE

* `req8`
* `req8 -e dev`
* `req8 city`
* `req8 -e dev city "GET collection"`

## SEE ALSO

[`.requests.yml` examples](./.requests.yml)

## AUTHOR

Rafael Bodill \<gmail:justRafi\>

## LICENSE

GNU GPLv3 (c) 2017 Rafael Bodill
