# ECD Helm chart

Helm chart to set up an empty EC.

Configure networking, auto-scaling and workflows in values.yaml

Deploy to cluster using helm command:

`helm upgrade --install my-ecd mediationzone-ecd`

To verify that resources are correctly deployed:

* kubectl describe ecd my-ecd


