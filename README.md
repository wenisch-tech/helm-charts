# Wenisch Tech Helm Charts

[![Helm repository](https://github.com/wenisch-tech/helm-charts/actions/workflows/build.yaml/badge.svg)](https://github.com/wenisch-tech/helm-charts/actions/workflows/build.yaml)

This repository hosts packaged Helm charts published by [Wenisch Tech](https://wenisch.tech). It is intended to be consumed as a Helm chart repository; chart source code and application documentation may live in their respective project repositories.

Repository URL: <https://charts.wenisch.tech>

## Usage

Add the repository and refresh its index:

```shell
helm repo add wenisch-tech https://charts.wenisch.tech
helm repo update
```

List the available charts and versions:

```shell
helm search repo wenisch-tech
helm search repo wenisch-tech --versions
```

Inspect a chart's default configuration:

```shell
helm show values wenisch-tech/<chart>
```

Install a chart:

```shell
helm install <release> wenisch-tech/<chart> \
  --namespace <namespace> \
  --create-namespace
```

To install a specific chart version, add `--version <version>`.


## Support

For chart-specific configuration and application behavior, consult the project links in the chart metadata:

```shell
helm show chart wenisch-tech/<chart>
```

For repository-index or publication issues, open an issue in this repository.
