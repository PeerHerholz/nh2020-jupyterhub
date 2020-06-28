![deploy-gke](https://github.com/neurohackademy/nh-2020/workflows/deploy-gke/badge.svg)
![deploy-book](https://github.com/neurohackademy/nh-2020/workflows/deploy-book/badge.svg)

# Infra and docs for hub.neurohackademy.org

hub.neurohackademy.org is a JupyterHub to be used by instructors and students of
the NeuroHackademy.org course 2020.

## Infrastructure

The Helm chart in [chart](chart) is automatically built and deployed in a GKE
cluster using [.github/workflows/deploy-gke](github/workflows/deploy-gke).
[mozilla/sops](https://github.com/mozilla/sops) and
[yuvipanda/hubploy](https://github.com/yuvipanda/hubploy) are tools used to do
this.

## Documentation

Documentation about this infrastructure is automatically built and published at
https://neurohackademy.github.io/nh-2020/ using
[.github/workflows/deploy-book](github/workflows/deploy-book) and the
documentation in [book](book) built with
[jupyter-book](https://github.com/executablebooks/jupyter-book).
