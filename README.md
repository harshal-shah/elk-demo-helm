## Description
This repo will set up Fluentd (for capturing logs from /var/lib/docker/containers) and forward them to elasticsearch and kibana.

## Important Note: 
If working on GKE, start your cluster with "Stackdriver Logging" disabled as fluentd installed by stackdriver will not work with elastic search provided from outside.

## Steps to run

Create helm release using following command: 
`helm install --name elk-chart ./elk-demo-helm`