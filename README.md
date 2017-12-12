This repository provides both `helmns` and `helmls` tools.

**`helmns`** `helm` cli wrapper forcing `--tiller-namespace` to match kubectl context

**`helmls`** a small script to list Helm releases across all `--tiller-namespaces`

# helmns

`helmns` is a [Helm](http://helm.sh) cli wrapper forcing `--tiller-namespace` to match kubectl context.

This is meant to simplify management for Kubernetes clusters with RBAC enabled and where tiller is heavily locked down per namespace.

# helmls

`helmls` is a small script to list Helm releases across all `--tiller-namespaces`.

-----

## Installation

Since `helmns` and `helmls` are written in Bash, they can run in shells that support POSIX standards.

- Download the `helmns` and `helmls` scripts
- Either:
  - save all somewhere in your `PATH`,
  - or save to a directory, then create symlinks from somewhere in your `PATH`, like `/usr/local/bin`
- Make scripts executable (`chmod +x ...`)

-----

Heavily based on [ahmetb/kubens](https://github.com/ahmetb/kubectx)
