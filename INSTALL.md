
Clone project


```shell
mkdir -p /srv
cd /srv
git clone https://github.com/LCSB-BioCore/gPAS.git
cd /srv/gPAS/docker/standard
```


Configure


```shell
cp httpd/mosaic.conf.template httpd/mosaic.conf
# edit settings
vim httpd/mosaic.conf
cp .env.template .env
# edit settings
vim .env
```

SSL (Optionnal)

```shell
Change certificates in `httpd` directory
```


Deploy

```shell
docker-compose up -d
```