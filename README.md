# docker-phpmd

## Download

```bash
$ docker pull mitakeck/phpmd
```

## Usage

```bash
$ docker run \
  -v `pwd`:/src \
  mitakeck/phpmd [<options>]
```

```bash
$ docker run -v `pwd`:/src mitakeck/phpmd src text codesize,unusedcode,design,naming
```
