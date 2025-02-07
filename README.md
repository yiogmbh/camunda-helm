# Camunda Helm
[![](https://img.shields.io/badge/Community%20Extension-An%20open%20source%20community%20maintained%20project-FF4700)](https://github.com/camunda-community-hub/community) [![Artifact HUB](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/camunda)](https://artifacthub.io/packages/search?repo=camunda)

Camunda public Kubernetes Helm repo and charts.

> **Note**
>
> This repo is a community effort for **Camunda Platform 7**, if you are looking for the brand new Camunda platform
> then go to the official [**Camunda Platform 8** Helm repo](https://github.com/camunda/camunda-platform-helm).


> **Note (yio gmbh)**
> 
> We forked this repository as we run it on a more recent kubernetes version using the stable ingress
> version (using especially *io.k8s.api.networking.v1.IngressBackend* api).
> This requires changes to the ingress templates. At the moment we do not have time to create
> syntax having backwards compatibility, so we forked the repository.
> We plan to bring changes back upstream, as soon as we have time to create a high quality solution.

## Repository

```sh
$ helm repo add camunda https://helm.camunda.cloud
$ helm repo update
```

## Charts

* [Camunda BPM Platform](./charts/camunda-bpm-platform)

## CI/CD

The CI/CD are done in GitHub Actions, and main actions are used:

* Testing charts via Helm [chart-testing-action](https://github.com/helm/chart-testing-action).
* Validating charts with different Kubernetes versions via [kind-action](https://github.com/helm/kind-action).
* Releasing charts via Helm [chart-releaser-action](https://github.com/helm/chart-releaser-action).

## Project status

Please note, this project still in under development, and could be there breaking changes but it will follow the SemVer convention.

## Contributing
We value all feedback and contributions. If you find any issues or want to contribute,
please feel free to [fill an issue](https://github.com/camunda-community-hub/camunda-helm/issues),
or [create a PR](https://github.com/camunda-community-hub/camunda-helm/pulls).

## License
This is open source software licensed using the Apache License 2.0. Please see [LICENSE](LICENSE) for details.
