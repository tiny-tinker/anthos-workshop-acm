# Anthos Config Management Root

Enabling Kubernetes operators to enforce configurations and policies on managed clusters.

This repo contains:

* `cluster`
   * `banned-key-template.yaml` - Gatekeeper constraint template. Defines the rule to enforce and what to say when triggered.
   * `banned-key-constraint.yaml` - Define when to enforce the constraint. This prevents secrets in `ConfigMap`s
   * `must-have-cust.yaml` - Deployments must have a customer label.
* `namespaces`
   * `app1-ns`/`namespace.yaml` - Adds the `app1-ns` namespace to the managed cluster(s).
   * `limit-range.yaml` - Example of limiting the resources for a container and persistent volume.
* `system`
   * `repo.yaml` - Defines this ACM repo.


