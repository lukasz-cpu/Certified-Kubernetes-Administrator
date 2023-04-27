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

3. What is the difference between NoExecute, NoSchedule, PreferNoSchedule?

https://stackoverflow.com/questions/50966318/what-is-the-difference-between-noexecute-noschedule-prefernoschedule

4. How to check if node is tainted? 

k describe node node01 | grep -i taints

5. How to add tolerations?

https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/

6. How to remove taint?

kubectl taint nodes controlplane node-role.kubernetes.io/control-plane:NoSchedule-

