# ansible_sample_db
ansibleを使ったpostgresqlインストールのサンプルです。

# how to use 

you install vagrant VM and execute provision.
```
$ vagrant up
```

2. you execute this command
```
$ bash after_vagrant_setup.sh
```
you will need to type valut.

3. install roles
```
$ ansible-galaxy install -r requirements.yml -p ./roles
```

4.execute ansible via playbook! and install app
```
$ ansible-playbook -i inventory.ini playbook.yml --ask-vault-pass
```
