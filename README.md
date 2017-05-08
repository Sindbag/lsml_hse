# LSML HSE course repo

## Azure notes

Before creating resources pull the latest version of scripts from the repository.

Update Azure CLI 2.0 to the latest verion:
`az component update`

Stop (deallocate) resources when you don't need them.

### To recreate cluster:
```
python cluster_control.py —user student* —remove
python create_cluster.py —user student* —ssh_key ~/.ssh/*.pub
```

Then continue with instructions in [How to create a Hadoop cluster](azure/docs/CREATE_CLUSTER.md) (skipping create_cluster.py, you've just done it).