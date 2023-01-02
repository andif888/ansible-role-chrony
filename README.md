# ansible-role-chrony

Role to install chrony.

## Table of content

- [Default Variables](#default-variables)
  - [chrony_all](#chrony_all)
  - [chrony_allow](#chrony_allow)
  - [chrony_ntp_pools](#chrony_ntp_pools)
  - [chrony_ntp_servers](#chrony_ntp_servers)
  - [chrony_service_name](#chrony_service_name)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Default Variables

### chrony_all

ip prefixed which are allow to use this server as time server

Example:

chrony_allow: ["192.168.0.0/24", "192.168.1.0/24"]

### chrony_allow

#### Default value

```YAML
chrony_allow: []
```

### chrony_ntp_pools

chrony configuration: ntp pools

#### Default value

```YAML
chrony_ntp_pools:
  - ntp.ubuntu.com        iburst maxsources 4
  - 0.ubuntu.pool.ntp.org iburst maxsources 1
  - 1.ubuntu.pool.ntp.org iburst maxsources 1
  - 2.ubuntu.pool.ntp.org iburst maxsources 2
```

### chrony_ntp_servers

chrony configuration: ntp servers

#### Default value

```YAML
chrony_ntp_servers: []
```

### chrony_service_name

chrony service name

#### Default value

```YAML
chrony_service_name: chronyd
```



## Dependencies

None.

## License

license (GPL-2.0-or-later, MIT, etc)

## Author

andif888
