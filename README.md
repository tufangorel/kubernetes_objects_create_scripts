## kubernetes_objects_create_scripts

### Tech Stack
Docker <br/>
Minikube <br/>
VS Code <br/>
Git Bash <br/>

### Run in the following order from terminal :

<pre>
$ kubectl apply -f pod.yaml
$ kubectl apply -f deployment.yaml
$ kubectl apply -f replicaset.yaml
$ kubectl apply -f service.yaml
$ kubectl apply -f ingress.yaml
$ kubectl create cm my-config --from-env-file=configs/some.properties
$ kubectl apply -f deployment-configuration.yml
$ kubectl apply -f secrets/myboot-deployment.yaml
$ kubectl apply -f secrets/myboot-service.yaml
$ kubectl create secret generic mysecret --from-literal=user='MyUserName' --from-literal=password='mypassword'
$ kubectl describe secret mysecret
$ kubectl get secret mysecret -o yaml
$ echo 'bXlwYXNzd29yZA==' | base64 --decode
$ echo 'TXlVc2VyTmFtZQ==' | base64 --decode
$ kubectl replace -f secrets/myboot-deployment-configuration-secret.yaml
$ kubectl delete deployment myboot
$ kubectl delete service myboot
</pre><br/>
