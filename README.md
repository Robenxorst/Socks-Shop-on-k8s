## Socks-Shop-on-k8s
Description of the name space of the k8s cluster responsible for the deployment of a website for the sale of socks.
## Running the Code
To run the site, you must have your own k8s cluster. In the beginning, clone this repository to the machine from which you administer k8s. In each `.yaml` file, change the namespace to your own. In the `ingress-front-end.yaml` change the domain name to the one you need.Once you have this repository on your machine, `cd` into the repository's root directory and run the following commands from the command line:
```
> kubectl create -k ./
```
## Required resources
To launch the site, you will need the following amount of resources:
`requests.cpu: 1/1`, `requests.memory: 1814Mi/2Gi`, `limits.cpu: 1900m/3`,
`limits.memory: 3628Mi/4Gi`
To find out the amount of resources consumed, use the command:
```
> kubectl get resourcequotas
```
