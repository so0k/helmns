# Helmns

helmns is a [Helm](http://helm.sh) cli wrapper forcing `--tiller-namespace` to match kubectl context.

This is meant to simplify management for Kubernetes clusters with RBAC enabled and where tiller is heavily locked down per namespace.

-----

## Installation

Since `helmns` is written in Bash, it can run in shells that support POSIX standards.

- Download the `helmns` script
- Either:
  - save to somewhere in your `PATH`,
  - or save to a directory, then create symlinks to `helmns` from somewhere in your `PATH`, like `/usr/local/bin`
- Make `helmns` executable (`chmod +x ...`)

-----

Heavily based on [ahmetb/kubens](https://github.com/ahmetb/kubectx)
