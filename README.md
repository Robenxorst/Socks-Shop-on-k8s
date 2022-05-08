## Socks-Shop-on-k8s
Description of the name space of the k8s cluster responsible for the deployment of a website for the sale of socks.
## Running the Code
To run the site, you must have your own k8s cluster and a dospa to it. In the beginning, clone this repository to the machine from which you administer k8s. In each .yaml file, change the namespace to your own. In the ingress-front-end.yaml change the domain name to the one you need.Once you have this repository on your machine, `cd` into the repository's root directory and run the following commands from the command line:

```
> kubectl create -k ./
```
