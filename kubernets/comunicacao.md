`$ sudo kubectl get pods -n dev`

Esse foi o resultado do comando com o nome do pod:
```
NAME                     READY   STATUS    RESTARTS   AGE

myapp-58575ff564-8mkw8   1/1     Running   0          7m35s
```

Agora vou entrar nesse pod usando o comando:

`$ sudo kubectl exec -n dev --stdin --tty myapp-58575ff564-8mkw8 -- /bin/bash`

Aqui eu ja estou no bash do pod:
```
root@myapp-58575ff564-8mkw8:/#
```
Executtando o curl: 

`# curl cluster-hmg.hmg.svc.cluster.local:8080`

Resltado:

```
<!DOCTYPE html>
<html>
<head>
<title>Welcome to nginx!</title>
<style>
html { color-scheme: light dark; }
body { width: 35em; margin: 0 auto;
font-family: Tahoma, Verdana, Arial, sans-serif; }
</style>
</head>
<body>
<h1>Welcome to nginx!</h1>
<p>If you see this page, the nginx web server is successfully installed and
working. Further configuration is required.</p>

<p>For online documentation and support please refer to
<a href="http://nginx.org/">nginx.org</a>.<br/>
Commercial support is available at
<a href="http://nginx.com/">nginx.com</a>.</p>

<p><em>Thank you for using nginx.</em></p>
</body>
</html>
```