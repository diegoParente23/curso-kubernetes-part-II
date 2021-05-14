# Curso de Kubernetes Parte II

Neste curso vamos estudar sobre `Deployment`, `Volumes` e `Escalabilidade`.

## Comandos importantes

```bash
# Retorna os replicasets ativos no momento
kubectl get replicasets
kubectl get rs
```

```bash
# Lista todos os deployments ativos
kubectl get deployments
```

```bash
# Lista o histórico de rollouts dado um deployment
kubectl rollout history deployment <DEPLOYMENT_NAME>
```

```bash
# Aplica as configs do arquivo gravando o deployment
kubectl apply -f <FILE_PATH> --record
```

```bash
# Aplica uma anotação ao deploy aplicado
kubectl annotate deployment <DEPLOYMENT_NAME> kubernetes.io/change-cause="<MESSAGE>"
```

```bash
# Realiza rollback de um deploy dado a sua revision id
kubectl rollout undo deployment <DEPLOYMENT_NAME> --to-revision=<REVISION_ID>
```
