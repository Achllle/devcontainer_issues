# minimally reproducible example of devcontainer/cli#904

[#904](https://github.com/devcontainers/cli/issues/904)

1. git clone this repo, open in vscode with dev containers extension installed (v0.384.0)
2. build the `original_container`
3. copy the resulting image hash
4. fill that in the [.devcontainer/compose_container/docker-compose.yml](.devcontainer/compose_container/docker-compose.yml) file under `image`
5. reopen in container, select `compose_container`
6. get the following error:

```bash
services.devcontainerissues.environment.[2]: unexpected type map[string]interface {}
```
