**[DEPRECATED] This repository is no longer maintained**
> While this project is fully functional, the content is no longer maintained and therefore is no longer up to date. You are still welcome to explore, learn, and use the code provided here.

# Solr Box

![No longer maintained](https://img.shields.io/badge/maintenance-OFF-red.svg?&style=flat-square)

Packer templates to build a Vagrant Solr box.

## Synopsis

This script will create a Vagrant box with Solr installed and with all of
the required libraries.

The box also has Zookeeper installed.

## Getting Started

There are a couple of things needed for the templates to work.

### Prerequisites

Packer tools need to be installed on your local computer.

#### Packer

Packer installation instructions can be found [here](https://www.packer.io/docs/installation.html).

#### Vagrant

Vagrant installation instructions can be found [here](https://www.vagrantup.com/docs/installation/).

#### Virtualbox

Virtualbox installation instructions can be found [here](https://www.virtualbox.org/wiki/Downloads).

### Installation

Nothing special to be done. Just download the template that you wish to use.

### Usage

In order to create the box using this packer script you need to provide a
few options.

```
Usage:
  packer build [-var 'option=value'] solr.json
```

#### Script Options
- `app_name` - The application name (default value: "solr").
- `app_name_ext` - Extra name for the application (default value: "").
- `headless` - Show the console of the machine being built (default value: "true").
- `java_build_number` - Java build number (default value: "11").
- `java_major_version` - Java major version (default value: "8").
- `java_token` - Java link token (default version: "d54c1d3a095b4ff2b6607d096fa80163").
- `java_update_version` - Java update version (default value: "131").
- `solr_version` - Solr version (default value: "6.4.0").
- `system_disk_size` - Size of the disk in MB (default value: "8192").
- `system_domain` - Domain name (default value: "marsh").
- `system_hostname` - Host name (default value: "solr").
- `system_locale` - Locale for the system (default value: "en_US").
- `system_pwd` - Password for the root and system users (default value: "solr").
- `system_timezone` - Time zone for the system (default value: "Europe/Lisbon").
- `system_user` - Username of the system user (default value: "pollywog").
- `zookeeper_version` - Zookeeper version (default value: "3.4.9").

## Services

This box will have the following services running.

| Service      | Port      | Protocol |
|--------------|:---------:|:--------:|
| SSH          | 22        |    TCP   |
| Zookeeper    | 2181      |    TCP   |
| Zookeeper    | 2888:3888 |    TCP   |
| Solr         | 8983      |    TCP   |

## Contributing

Contributing to this project is no longer possible since the project is no
longer maintained.

## Versioning

This project uses [SemVer](http://semver.org/) for versioning. For the versions
available, see the [tags on this repository](https://github.com/fscm/packer-vagrant-solr/tags).

## Authors

* **Frederico Martins** - [fscm](https://github.com/fscm)

See also the list of [contributors](https://github.com/fscm/packer-vagrant-solr/contributors)
who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE)
file for details
