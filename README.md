## CoreDNS Docker Compose

#### Configurables
- `group_vars/all.yaml`

| Value | Description | Default |
| :---        |    :----   |          ---: |
| docker.user | User to run containers under | ubuntu |
| optional_tasks.setup_compose | Create media stack directory structure and containers | enabled |
| optional_tasks.compose_basedir | Base directory to create the media_stack sub directories under | docker |
| optional_tasks.restartPolicy | Configure how Docker starts containers on boot | unless-stopped |
| optional_tasks.setup_docker_zfs | Create a ZFS dataset for Docker directories | disabled |

_Tested on amd64 Ubuntu 22.04 LTS_
