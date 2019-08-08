# kubernetes-ELK
https://www.digitalocean.com/community/tutorials/how-to-set-up-an-elasticsearch-fluentd-and-kibana-efk-logging-stack-on-kubernetes

1. kubectl create -f https://raw.githubusercontent.com/RedxLus/kubernetes-ELK/master/elasticsearch_svc.yaml
kubectl get services

2. kubectl create -f https://raw.githubusercontent.com/RedxLus/kubernetes-ELK/master/elasticsearch_statefulset.yaml
kubectl rollout status sts/es-cluster
kubectl port-forward es-cluster-0 9200:9200

3. 
