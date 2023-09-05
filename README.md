|![](https://upload.wikimedia.org/wikipedia/commons/thumb/1/17/Warning.svg/156px-Warning.svg.png) | This project is no longer supported.
|---|---|

# Helm Charts

This GitHub project is the source for Helm charts used by Hireflix.

For more information about installing and using Helm, see the
[Helm Docs](https://helm.sh/docs/). For a quick introduction to Charts, see the [Chart Guide](https://helm.sh/docs/topics/charts/).

For issues and support for Helm and Charts see [Support Channels](CONTRIBUTING.md#support-channels).

## How Do I Install These Charts?

Just `helm install hireflix/<chart>`.

For more information on using Helm, refer to the [Helm documentation](https://github.com/kubernetes/helm#docs).

## How Do I Enable the Stable Repository for Helm 3?

To add the Helm Stable Charts for your local client, run `helm repo add`:

```
$ helm repo add hireflix https://hireflix.github.io/charts
"stable" has been added to your repositories
```

## Chart Format

Take a look at the [alpine example chart](https://github.com/helm/helm/tree/master/cmd/helm/testdata/testcharts/alpine) for reference when you're writing your first few charts.

Before contributing a Chart, become familiar with the format. Note that the project is still under active development and the format may still evolve a bit.

## Repository Structure

This GitHub repository contains the source for the packaged and versioned charts released using [GitHub pages](https://github.com/helm/charts/tree/gh-pages/stable) (the Chart Repository).

The Charts in the `stable/` directory in the master branch of this repository match the latest packaged Chart in the Chart Repository, though there may be previous versions of a Chart available in that Chart Repository.

The purpose of this repository is to provide a place for maintaining and contributing official Charts, with CI processes in place for managing the releasing of Charts into the Chart Repository.

The Charts in this repository are organized into one folder:

* stable

Stable Charts meet the criteria in the [technical requirements](CONTRIBUTING.md#technical-requirements).

## Contributing to an Existing Chart

We'd love for you to contribute to an existing Chart that you find provides a useful application or service for Kubernetes. Please read our [Contribution Guide](CONTRIBUTING.md) for more information on how you can contribute Charts.

Note: We use the same [workflow](https://github.com/kubernetes/community/blob/master/contributors/devel/development.md#workflow),
[License](LICENSE) and [Contributor License Agreement](CONTRIBUTING.md) as the main Kubernetes repository.