## Ansible postgres_basic

Ansible role which installs and configures basic standalone PostgreSQL from Ubuntu repository.

WARNING: This doesn't deal with character encoding, you need to take care of this before creating DBs
         See: https://github.com/knopki/ansible-locale


#### Installation

This has been tested on Ansible 1.9.4 and higher.

To install:

```
git clone 
```

#### Variables

```yaml
postgresql_dbname: foo
postgresql_dbuser: foo
postgresql_dbpassword: verysecretpassword

```


#### Testing
This project comes with a Vagrantfile, this is a fast and easy way to test changes to the role, fire it up with `vagrant up`

See [vagrant docs](https://docs.vagrantup.com/v2/) for getting setup with vagrant

Once your VM is up, you can reprovision it using either `vagrant provision`, or `ansible-playbook tests/playbook.yaml -i inventory`

You will need to provide some jar file in order this to work though. You can do it manually by ssh-ing into box: `vagrant ssh`

Directory with `Vagrantfile` is being mounted automatically so you can just copy jar file manually or add it to playbook.yaml file

#### License

Licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.


