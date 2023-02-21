# portable-skyrim

* Source for website
* Requires mkdocs to build
* Homepage: https://portable-skyrim.info/

## Build site

```
$ mkdocs build
```

## Deploy site

```
$ cd ansible
$ ansible-playbook -i inventory.yaml --limit hosttech portable-skyrim-website.yaml
```

## Webserver setup

* Host: 35923.hostserv.eu
* /data/docker-compose/web/

* Restart webserver:

```
$ docker-compose down
$ docker-compose up -d
```

* Admin frontproxy login: 

https://admin.retro-io.com
