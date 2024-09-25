This is not ready to be applied in any environment the purpose is to show the capabilities of using kustomization apply changes into kubernetes deployment.
In order to test it, 
just go to the folders 
overlays/dev or overlays/prd

> kustomize build .

in future to apply it in an environment 

> kubectl apply -k . 

For the app1 kustomiation to build

> kustomize build . --load-restrictor LoadRestrictionsNone

This makes brakes the self containability of the kustomization files but allows us to reuse config, yamls and secretes.
