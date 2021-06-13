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
$ kubectl create namespace pizzahat
$ kubectl config set-context --current --namespace=pizzahat
$ kubectl apply -f crds/pizza-crd.yaml
$ kubectl get crds | grep pizza
$ kubectl api-resources | grep pizzas
$ kubectl apply -f crds/pizza-deployment.yaml
$ kubectl get pods
$ kubectl apply -f crds/cheese-pizza.yaml
$ kubectl get pizzas
$ kubectl describe pizza cheesep
$ kubectl get pods
$ kubectl logs cheesep-pod
$ kubectl apply -f crds/meat-pizza.yaml
$ kubectl apply -f crds/veggie-lovers.yaml
$ kubectl get pizzas --all-namespaces
$ kubectl delete pizzas --all
$ kubectl delete all --all
$ kubectl delete namespace pizzahat
$ kubectl delete -f crds/pizza-crd.yaml
$ kubectl apply -f volumes/myboot-pod-volume.yaml
$ kubectl get pods
$ kubectl delete pod myboot-demo
$ kubectl apply -f volumes/myboot-pods-volume.yaml
$ kubectl describe pod myboot-demo
$ kubectl delete -f volumes/myboot-pods-volume.yaml
$ kubectl apply -f volumes/myboot-pod-volume-hostpath.yaml
$ kubectl describe pod myboot-demo
$ kubectl delete pod myboot-demo
$ kubectl apply -f volumes/demo-persistent-volume-hostpath.yaml
$ kubectl get pv
$ kubectl apply -f volumes/myboot-persistent-volume-claim.yaml
$ kubectl get pvc
$ kubectl apply -f volumes/myboot-pod-volume-pvc.yaml
$ kubectl describe pod myboot-demo
$ kubectl delete pod myboot-demo
$ kubectl get pvc
$ kubectl delete -f volumes/myboot-persistent-volume-claim.yaml
$ kubectl delete -f volumes/demo-persistent-volume-hostpath.yaml
$ kubectl get sc
$ kubectl apply -f volumes/demo-dynamic-persistent.yaml
$ kubectl apply -f volumes/myboot-pod-volume-pvc.yaml
$ kubectl get pods
$ kubectl get pvc
$ kubectl get pv
$ kubectl delete -f volumes/myboot-pod-volume-pvc.yaml
$ kubectl delete -f volumes/demo-dynamic-persistent.yaml
$ kubectl apply -f jobs/whalesay-job.yaml
$ kubectl get pods
$ kubectl get jobs
$ kubectl logs whale-say-job-wbp4c
$ kubectl delete -f jobs/whalesay-job.yaml
$ kubectl apply -f cronjobs/whalesay-cronjob.yaml
$ kubectl get pods
$ kubectl get cronjobs
$ kubectl get pods
$ kubectl get jobs
$ kubectl delete -f cronjobs/whalesay-cronjob.yaml
$ kubectl apply -f daemonsets/quarkus-daemonset.yaml
$ kubectl get pods -o wide
$ kubectl delete -f daemonsets/quarkus-daemonset.yaml
$ kubectl apply -f statefulsets/quarkus-statefulset.yaml
$ kubectl get pods
$ kubectl get statefulsets
$ kubectl scale statefulset quarkus-statefulset --replicas=3
$ kubectl get pods
$ kubectl get events --sort-by=.metadata.creationTimestamp
$ kubectl scale statefulset quarkus-statefulset --replicas=2
$ kubectl get pods
$ kubectl delete -f statefulsets/quarkus-statefulset.yaml

</pre><br/>
