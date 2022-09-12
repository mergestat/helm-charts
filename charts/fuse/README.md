# `fuse`

This is the helm chart for the [`mergestat/fuse`](https://github.com/mergestat/fuse) project.
There are three main components to a Fuse deployment:

1. PostgreSQL database
2. Backend worker(s)
3. User interface (and GraphQL API)

The default values in `values.yaml` *should* be sufficient to deploy an instance and get started, though some values may need to be overridden.

This chart includes the [`bitnami/postgresql`](https://github.com/bitnami/charts/tree/master/bitnami/postgresql) chart (driven by `postgresql.enabled`) as a subchart, though you may use any PostgreSQL instance made accessible to the pods in this chart.
