# batchsftpcollect

This demo shows how to ... The workflow:

***Pulse --> Analysis --> Aggregation --> Prometheus***


| Agent  | Description |
| ------------- | ------------- |
| Pulse        | Activates data generation (once per second).  |
| Analysis     | Creates data. Each record represents some sold volume for a specific country.  |
| Aggregation  | Aggregates total sold volumes per country.  |
| Prometheus   | Forwards aggregates records to Promethus for storage.  |


### Import / Deploy

To import the workflow example use the mzcli command line tool

`mzcli <user>/<password> systemimport <export-dir>`

To deploy in Kubernetes using the ECD resource

`kubectl apply -f <resource.yaml>`

To verify that resources are correctly deployed:

* login to MZOnline web UI and monitor the resources in the EC Deployment view
*or*
* Use kubectl to check installed ECD resources: `kubectl describe ecd <example-name>`



