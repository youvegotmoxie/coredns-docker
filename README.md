## CoreDNS Docker Compose

#### Configurables
- `group_vars/all.yaml`

#### Prerequisites for installing the Datadog agent (optional)
- `ansible-galaxy install datadog.datadog`
- Configure `group_vars/datadog.yaml`
- Create the `group_vars/datadog-api.yaml` file that contains a variable `dd_api_key` with your Datadog API key

| Value | Description | Default |
| :---        |    :----   |          ---: |
| docker.user | User to run containers under | ubuntu |
| optional_tasks.setup_compose | Create directory structure for containers | enabled |
| optional_tasks.compose_basedir | Base directory to create the coredns sub directories under | docker |
| optional_tasks.restartPolicy | Configure how Docker starts containers on boot | unless-stopped |

_Tested on amd64 Ubuntu 22.04 LTS_
