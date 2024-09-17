https://kubernetes.io/docs/tasks/manage-kubernetes-objects/kustomization/
This is not ready to be applied in any environment the purpose is to show the capabilities of using kustomization apply changes into kubernetes deployment.
In order to test it, 
just go to the folders 
overlays/dev or overlays/prd

> kustomize build .

in future to apply it in an environment 

> kubectl apply -k . 