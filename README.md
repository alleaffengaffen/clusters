# clusters
Repo containing all Cluster definitions.

Do separate cluster we use a new Argo CD for each cluster.

`clusters.yaml` is the App of Apps that reads the `apps` directory.
`apps` contains a bunch of `kind:Application` yamls that each point to another folder in this repo.

## Cluster API

We use cluster-api to provision those clusters. Here's a list of the currently enabled providers you can use:

Enabled providers:
- AWS (eu-west-2)
