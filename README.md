# Syno_Docker-PiHole
Run PiHole with Synology Docker.<br>
 
&nbsp;<br>
[
    ![Open source](
        https://img.shields.io/badge/Open%20Source-Yes-green?style=plastic
    )
    ](
        https://github.com/dannyvanlierop/Syno_Docker-PiHole
    )
[
    ![License: Mit](
        https://img.shields.io/badge/license-MIT-green.svg?style=plastic)
    ](
        https://en.wikipedia.org/wiki/MIT_License
    )
[
    ![Contributors](
        https://img.shields.io/github/contributors/dannyvanlierop/Syno_Docker-PiHole?style=plastic)
    ](
        https://github.com/dannyvanlierop/Syno_Docker-PiHole/graphs/contributors
    )
[
    ![Forks](
        https://img.shields.io/github/forks/dannyvanlierop/Syno_Docker-PiHole?style=plastic)
    ](
        https://github.com/dannyvanlierop/Syno_Docker-PiHole/network/members
)
[
    ![Stars](
        https://img.shields.io/github/stars/dannyvanlierop/Syno_Docker-PiHole?style=plastic)
  ](
        https://github.com/dannyvanlierop/Syno_Docker-PiHole/stargazers
)
[
    ![Issues](
        https://img.shields.io/github/issues/dannyvanlierop/Syno_Docker-PiHole?style=plastic)
  ](
        https://github.com/dannyvanlierop/Syno_Docker-PiHole/issues
)

&nbsp;<br>
## Extract zip files:
<hr>

```
./syno_docker-pihole_v01.zip.001
./syno_docker-pihole_v01.zip.002
```

&nbsp;<br>
## Import extracted Image, 
<hr>

```
docker image import ./syno_docker-pihole_v01
```

&nbsp;<br>
## Configure container:
<hr>

```
-RunAs root
-Enable autostart
```

&nbsp;<br>
## Mount folders:
<hr>

```
/etc/pihole
/etc/dnsmasq.d
```

&nbsp;<br>
## Configure environment variables and start container:
<hr>

```
SKIPGRAVITYONBOOT = True or False
WEB_PORT          = 8080 or other
WEBPASSWORD       = PiHole Password.
DNSMASQ_LISTENING = local
ServerIp          = IP docker server
```

&nbsp;<br>
## List containers:
<hr>

```
docker container ls
```

&nbsp;<br>
## Connect to container terminal:
<hr>

```
docker exec -lt [CONTAINER_ID] bash
```

&nbsp;<br>
## List current images:
<hr>

```
docker images
```

&nbsp;<br>
## Commit listed imageID to imageName:
<hr>

```
docker commit [CONTAINER_ID] [NEW_IMAGE_NAME]
docker commit 4d5aa143901a syno_docker-pihole_v01:latest
```

&nbsp;<br>
## Save the new file:
<hr>

```
docker image save -o PATH_TO_IMAGE/NEW_IMAGE_NAME [NEW_IMAGE_NAME]
```

&nbsp;<br>
## Dependency:
<hr>

- [docker](https://https://www.docker.com/company)<br>
- [blocklistproject](https://github.com/blocklistproject.com)<br>

&nbsp;<br>
## License:
<hr>

For more details,
see the [LICENSES](https://github.com/dannyvanlierop/NodeJS_HueBridge-Mirror-API/blob/master/LICENSE) file.

<br>&nbsp;

