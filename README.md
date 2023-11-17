# all_about_shell

This repositoy contains all the useful shells and bash alias I have been using
- alias
  - Kubernetes
    - ```alias k=kubectl```
    - ```alias kubectx="kubectl ctx"```
  - virsh
    - ```alias virshnet="virsh net-dhcp-leases default"```
  - Linux command
    - ```alias dir_size="du --max-depth=1 -h | sort -h"```
    - ```alias du_depth="du --max-depth=1 -h"```
    - ```alias du_sort="du -h | sort -h```
- shell
  - Kubernetes
  - SLATE
  - 

- Useful .bashrc
  ```bash
  HISTSIZE=20000
  HISTFILESIZE=20000
  ```

## Docker
**problem**
```bash
$ docker ps
ERROR: permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/_ping": dial unix /var/run/docker.sock: connect: permission denied
permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Post "http://%2Fvar%2Frun%2Fdocker.sock/v1.24/images/ghcr.io/adiprerepa/slate-plugin/push?tag=latest": dial unix /var/run/docker.sock: connect: permission denied
```
**solution**
```bash
sudo chmod 666 /var/run/docker.sock
```
