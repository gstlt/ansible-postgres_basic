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

When done, invoke `vagrant destroy` command.

#### License

Licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.


