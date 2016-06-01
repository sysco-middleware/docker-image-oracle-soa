# Docker Image: Oracle SOA Suite

Image with Oracle SOA Suite installed.

## Base image

syscomiddleware/oracle-database-instant-client

## Ansible roles

- sysco-middleware.oracle-soa

> ansible-galaxy install -f sysco-middleware.oracle-soa

## How to build it

Define installers path:

```yaml
volumes:
  - "/opt/installers/oracle/fmw/12.1/soa-qs/12.1.3:/srv/files"
```

Make sure to unzip installers in this directory.

And run:

> ansible-playbook main.yml

## Tags

- soa-qs-12.1.3-jdk7-centos7

- soa-qs-12.2.1-jdk8-centos7
