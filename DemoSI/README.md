# mz-example-workflows
Example workflows for MediationZone by DigitalRoute

The examples are designed to work on latest minor release MediationZone, installed on a Kubernetes cluster.

Each example consists of a workflow export directory and a directory containing a yaml resource file to deploy the example in a Kubernetes cluster.

To import the workflow example use the mzcli command line tool

`mzcli <user>/<password> systemimport <export-dir>`

To deploy in Kubernetes using the ECD resource

`kubectl apply -f <resource.yaml>`

To verify that resources are correctly deployed:

* login to MZOnline web UI and monitor the resources in the EC Deployment view
*or*
* Use kubectl to check installed ECD resources: `kubectl describe ecd <example-name>`
