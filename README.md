# docker-builders
docker images for python projects' CI

## lint

python linters: black, mypy ....

to be used in CI builders or to mutualise between local projects

linux
```bash
docker run --rm -it -v $PWD:/opt nlaurance/lint:3.9 bash
```
cygwin
```shell
docker run --rm -it -v $(cygpath -w $(pwd)):/opt nlaurance/lint:3.9 bash
```

## xmlsec

A python interpreter with support for xmlsec
as per https://pythonhosted.org/xmlsec/install.html