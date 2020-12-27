# Syno_Docker-PiHole
 Docker container with PiHole installed.<br>
 Configured with filters from https://github.com/blocklistproject.com<br>

[
    ![Open source](
        https://img.shields.io/badge/Open%20Source-Yes-green?style=plastic
    )
    ](
        https://github.com/dannyvanlierop/Syno_Docker-PiHole
    )
[
    ![License: Unlicense](
        https://img.shields.io/badge/license-Unlicense-blue.svg?style=plastic)
    ](
        http://unlicense.org/
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

&nbsp;
## Load container:
<hr>

#### Extract zip files:
```
./syno_docker-pihole_v01.zip.001
./syno_docker-pihole_v01.zip.00
```
#### Import extracted Image, or add image by file with DSM docker "Add from URL"
```
docker image import ./syno_docker-pihole_v01
```

#### Configure container:
```
-RunAs root
-Enable autostart
```

#### Mount folders:
```
/etc/pihole
/etc/dnsmasq.d
```

#### Configure environment variables:
```
SKIPGRAVITYONBOOT = True or False
WEB_PORT          = 8080 or other
WEBPASSWORD       = PiHole Password.
DNSMASQ_LISTENING = local
ServerIp          = IP docker server
```

#### Start the container, done

&nbsp;
## Save container:
<hr>

#### Change container

#### List containers
```
docker container ls
```

#### Connect to container terminal
```
docker exec -lt [CONTAINER_ID] bash
```

#### List current images
```
docker images
```

#### Commit listed imageID to imageName
```
docker commit [CONTAINER_ID] [NEW_IMAGE_NAME]
docker commit 4d5aa143901a syno_docker-pihole_v01:latest
```

#### Save the new file
```
docker image save -o PATH_TO_IMAGE/NEW_IMAGE_NAME [NEW_IMAGE_NAME]
```

#### Done.
