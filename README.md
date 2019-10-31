# Digitransit OKD deploy

## Prerequisites
* have Openshift v3.11 installed
* have oc cli installed

## Run
1. `oc cluster up`
2. `oc new-project <project name>`
3. `oc create -f services.yml,deployments.yml `
4. `oc status`