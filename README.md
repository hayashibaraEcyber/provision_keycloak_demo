# provision_keycloak_demo

develop dry run

```sh
cd ansible
sudo ansible-playbook -i develop keycloak.yml -u vagrant --ask-pass --ask-become-pass --check
```

production run

```sh
cd ansible
sudo ansible-playbook -i production keycloak.yml -u root --ask-pass --ask-become-pass
sudo ansible-playbook -i production web.yml -u root --ask-pass --ask-become-pass
```
