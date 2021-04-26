# Homework

Everything is very simple, you just need to set up group replication for the MySQL nodes spawned =)

## A small checklist before starting to do Homework

- Clone this repo
- Run `make uninstall` and `make install`
- Run `make deploy` and make sure that `namespace` has been created and our pod with the operator is launched in it
- Change the context so that `kubectl` will" look "into our namespace.
 `kubectl config set-context --current --namespace = NAMESPACE_NAME`
- We apply our custom resource. `kubectl apply -f config / samples / workshop_v1alpha1_custommysql.yaml`
- After that, 2 pods with mysql should rise (it may take some time, so don't rush here)
- After, look at the file `controllers / mysql.go`
- **IF SOMETHING GOES WRONG, WRITE TO CHAT)**
