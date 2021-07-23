## Cleanup

kubectl delete svc -n bearcanoe-root --all
kubectl delete svc -n steveslokadev-root --all           
kubectl delete deployment -n steveslokadev-root --all             
kubectl delete deployment -n bearcanoe-root --all             
kubectl delete proxy -A --all  
kubectl delete ns marketing