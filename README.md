# `Docker` using `Multipass`

- `Multipass` must be installed

#### Launch `Multipass` instance
```sh
source bin/launch-instance
```
or
```sh
multipass launch --cpus 4 --memory 4GB --disk 10GB --name docker 22.04 --cloud-init multipass-docker.yml
```

#### Kill `Multipass` instance
```sh
source bin/kill-instance
```
or
```sh
multipass delete docker
multipass purge
```

#### Access to the `Multipass` instance
```sh
multipass shell docker
```

#### List IP adrress of `Multipass` instance
```sh
multipass list
```

## References
- [multipass.run](https://multipass.run/)
- [Multipass Docs](https://multipass.run/docs)
