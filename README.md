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
</pre><br/>
