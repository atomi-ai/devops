# HOW TO DEPLOY WORDPRESS

先用下面的方式检查下k8s中的变化情况，
```shell
helm diff upgrade xfguo-wp . -n wp-exp -f values.yaml
```

然后用下面的命令upgrade当前的k8s wordpress配置。
```shell
helm upgrade xfguo-wp . -n wp-exp -f values.yaml
```
