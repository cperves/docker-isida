# Isida servers for Moodle question type plugins  modlsimilarity et reacsimilarity
## Install and run
### molsimilarity
* plugin can be found here https://moodle.org/plugins/qtype_molsimilarity
* to install server with docker image
```shell
docker pull ghcr.io/cperves/isida:1.7
docker container run --publish 9080:9080 --detach ghcr.io/cperves/isida:1.7
# server will run on 9080 port but you can chnage to another port --publish newport:9080
``` 
* in moodle molsimilarity plugin settings
  * change `qtype_molsimilarity | isidaurl` to http://servername:9080 or http://servername:newport

### readsimilarity
* plugin can be found here https://moodle.org/plugins/qtype_reacsimilarity
* to install server with docker image
```shell
docker pull ghcr.io/cperves/isidareac:1.7
docker container run --publish 9090:9090 --detach ghcr.io/cperves/isidareac:1.7
# server will run on 9080 port but you can change to another port --publish newport:9090
``` 
* in moodle reacsimilarity plugin settings
    * change `qtype_reacsimilarity | isidaurl` to http://servername:9090 or http://servername:newport

## Roadmap
[Roadmap](./ROADMAP.md)

## Change Log
[Change Log](./CHANGELOG.md)