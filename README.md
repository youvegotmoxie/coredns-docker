## CoreDNS Docker Compose

#### Configurables
- `group_vars/all.yaml`

#### Prerequisites
- `ansible-galaxy install datadog.datadog` _(optional install datadog agent)_
- Configure `group_vars/datadog.yaml`
- Create the `group_vars/datadog-api.yaml` file that contains a variable `dd_api_key` with your Datadog API key

| Value | Description | Default |
| :---        |    :----   |          ---: |
| docker.user | User to run containers under | ubuntu |
| optional_tasks.setup_compose | Create media stack directory structure and containers | enabled |
| optional_tasks.compose_basedir | Base directory to create the media_stack sub directories under | docker |
| optional_tasks.restartPolicy | Configure how Docker starts containers on boot | unless-stopped |

_Tested on amd64 Ubuntu 22.04 LTS_
