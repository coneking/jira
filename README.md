# Deploy Jira Kubernetes

- Clonar repositorio

```sh
$ git clone http://gitlab.cencosud.corp/SConejer/jira.git
```

<br>

- Deploy Jira

```sh
$ kubectl create ns jira
$ kubectl -n jira apply -f jira/k8s/prod/
```

<br>

- Verificar si el deployment de Jira fue exitoso.

```sh
$ kubectl -n jira get pvc,deploy,pod,svc,ing
```
