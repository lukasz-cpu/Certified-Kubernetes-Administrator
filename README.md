# Certified-Kubernetes-Administrator
Certified Kubernetes Administrator - Exam Notes

k = kubectl

1. How to get pods by label?

For example:
k get pods --selector env=dev
k get pods --selector bu=finance

2. 

If it possible to find resource using multiple selectors? 

kubectl get all --selector env=prod,bu=finance,tier=frontend


