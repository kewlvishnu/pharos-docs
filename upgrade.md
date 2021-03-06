# Upgrade Kontena Pharos Cluster

When new versions of Kontena Pharos are released, you can upgrade your existing cluster to apply the latest enhancements and bug fixes. This includes upgrading from previous minor versions, such as release 1.0 to 1.1, and applying asynchronous errata updates within a minor version (1.0.z releases). See the [Kontena Pharos Release Notes](https://github.com/kontena/pharos-cluster/releases) to review the latest changes.

Unless noted otherwise, worker and masters within a major version are forward and backward compatible across one minor version, so upgrading your cluster should go smoothly. Please note: downgrades are NOT supported!

## Upgrade Steps

### 1. Install new version of `pharos` CLI tool

Use `chpharos` to install and use new version of `pharos` CLI tool. For example install and use version 1.2.3 of Kontena Pharos:

```
$ chpharos install 1.2.3
$ chpharos use 1.2.3
```

HINT: You can see the list of all available versions using `chpharos list-remote` command.

### 2. Apply upgrade to your cluster

Once you have switched the `pharos` CLI tool to new version, simply run `pharos up` command with your cluster specific `cluster.yml` configuration file. For example:

```
$ pharos up -c cluster.yml
```

### 3. Enjoy!

We hope it was smooth experience. If you encounter any issues or trouble, please let us know!