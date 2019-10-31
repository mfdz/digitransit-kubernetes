# Digitransit OKD deploy

## Prerequisites
* have Openshift v3.11 installed
* have oc cli installed

## Run
1. `oc cluster up`
2. `oc new-project <project name>`
3. `oc login -u system:admin`
4. `oc adm policy add-scc-to-user anyuid <project_name> -z default`
5. `oc create -f services.yml,deployments.yml`
6. `oc status`