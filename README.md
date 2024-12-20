# PostgreSQL Extension Repo

[![Webite: ext.pigsty.io](https://img.shields.io/badge/website-ext.pigsty.io-slategray?style=flat&logo=cilium&logoColor=white)](https://ext.pigsty.io)
[![Extensions: 340](https://img.shields.io/badge/extensions-340-%233E668F?style=flat&logo=postgresql&logoColor=white&labelColor=3E668F)](https://pigsty.io/docs/pgext/list)

The supplementary [APT](#apt-repo) and [YUM](#yum-repo) repo for PostgreSQL extensions, maintained and used by [Pigsty](https://pigsty.io)

Provide 340 available [Extensions](https://ext.pigsty.io/#/list) as [RPM](https://ext.pigsty.io/#/rpm) / [DEB](https://ext.pigsty.io/#/deb) for PostgreSQL **12** - **17** in addition to the official PGDG repo.

Available on Linux: Debian 12 / Ubuntu 24.04 / 22.04 / EL8 / EL9 compatible OS distros, and `x86_64` & `ARM64` architectures.

| Entry / Filter | All | PGDG | PIGSTY | CONTRIB | MISC | MISS | PG17 | PG16 | PG15 | PG14 | PG13 | PG12 |
|:--------------:|:---:|:----:|:------:|:-------:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
| RPM Extension  | 334 | 115  |  143   |   70    |  4   |  6   | 301  | 330  | 333  | 319  | 307  | 294  |
| DEB Extension  | 326 | 104  |  144   |   70    |  4   |  14  | 302  | 322  | 325  | 316  | 303  | 293  |

**Why extension matters to PostgreSQL?** check the post: "[***PostgreSQL is eating the database world!***](https://medium.com/@fengruohang/postgres-is-eating-the-database-world-157c204dcfc4)"

[![PostgreSQL Extension Ecosystem](https://pigsty.io/img/pigsty/ecosystem.jpg)](https://medium.com/@fengruohang/postgres-is-eating-the-database-world-157c204dcfc4)

> [The idea way to deliver PostgreSQL extensions](https://medium.com/@fengruohang/the-idea-way-to-deliver-postgresql-extensions-35646464bb71)

-------

## Get Started

All rpm/deb packages are signed with GPG key `B9BD8B20` (`9592A7BC7A682E7333376E09E7935D8DB9BD8B20` ).

### APT Repo

[![Linux AMD](https://img.shields.io/badge/Linux-AMD64-%23FCC624?style=flat&logo=linux&labelColor=FCC624&logoColor=black)](https://pigsty.io/docs/node)
[![Linux ARM](https://img.shields.io/badge/Linux-ARM64-%23FCC624?style=flat&logo=linux&labelColor=FCC624&logoColor=black)](https://pigsty.io/docs/node)
[![Ubuntu Support: 24](https://img.shields.io/badge/Ubuntu-24-%23E95420?style=flat&logo=ubuntu&logoColor=%23E95420)](https://pigsty.io/docs/pgext/list/deb/)
[![Ubuntu Support: 22](https://img.shields.io/badge/Ubuntu-22-%23E95420?style=flat&logo=ubuntu&logoColor=%23E95420)](https://pigsty.io/docs/pgext/list/deb/)
[![Debian Support: 12](https://img.shields.io/badge/Debian-12-%23A81D33?style=flat&logo=debian&logoColor=%23A81D33)](https://pigsty.io/docs/reference/compatibility/)

For Ubuntu 22.04 & Debian 12 or any compatible platforms, use the following commands to add the APT repo:

```bash
curl -fsSL https://repo.pigsty.io/key | sudo gpg --dearmor -o /etc/apt/keyrings/pigsty.gpg
sudo tee /etc/apt/sources.list.d/pigsty-io.list > /dev/null <<EOF
deb [signed-by=/etc/apt/keyrings/pigsty.gpg] https://repo.pigsty.io/apt/infra generic main 
deb [signed-by=/etc/apt/keyrings/pigsty.gpg] https://repo.pigsty.io/apt/pgsql/$(lsb_release -cs) $(lsb_release -cs) main
EOF
sudo apt update
```

### YUM Repo

[![Linux](https://img.shields.io/badge/Linux-x86_64-%23FCC624?style=flat&logo=linux&labelColor=FCC624&logoColor=black)](https://pigsty.io/docs/node)
[![Linux Aarch64](https://img.shields.io/badge/Linux-Aarch64-%23FCC624?style=flat&logo=linux&labelColor=FCC624&logoColor=black)](https://pigsty.io/docs/node)
[![RHEL Support: 8/9](https://img.shields.io/badge/EL-7/8/9-red?style=flat&logo=redhat&logoColor=red)](https://pigsty.io/docs/pgext/list/rpm/)
[![RHEL](https://img.shields.io/badge/RHEL-slategray?style=flat&logo=redhat&logoColor=red)](https://pigsty.io/docs/pgext/list/rpm/)
[![CentOS](https://img.shields.io/badge/CentOS-slategray?style=flat&logo=centos&logoColor=%23262577)](https://almalinux.org/)
[![RockyLinux](https://img.shields.io/badge/RockyLinux-slategray?style=flat&logo=rockylinux&logoColor=%2310B981)](https://almalinux.org/)
[![AlmaLinux](https://img.shields.io/badge/AlmaLinux-slategray?style=flat&logo=almalinux&logoColor=black)](https://almalinux.org/)
[![OracleLinux](https://img.shields.io/badge/OracleLinux-slategray?style=flat&logo=oracle&logoColor=%23F80000)](https://almalinux.org/)

For EL 8/9 and compatible platforms, use the following commands to add the YUM repo:

```bash
curl -fsSL https://repo.pigsty.io/key      | sudo tee /etc/pki/rpm-gpg/RPM-GPG-KEY-pigsty >/dev/null  # add gpg key
curl -fsSL https://repo.pigsty.io/yum/repo | sudo tee /etc/yum.repos.d/pigsty.repo        >/dev/null  # add repo file
sudo yum makecache
```

-------

## What's Inside

Linux x86_64/amd64 [Extension](/list) packages for PostgreSQL 12 - 17, on El8, EL9, Ubuntu 22.04 and Debian 12.

Check the [extension list](https://ext.pigsty.io/#/list) for details.


----------------

## Contrib

If you have any suggestions on including new extensions or bumping to new versions, or find any mistake about metadata,
PR or [Issue](https://github.com/pgsty/extension/issues/new) are welcome!

You can edit the [`pigsty.csv`](https://github.com/pgsty/extension/blob/main/data/pigsty.csv) raw data and create a pull
request to update the metadata.


----------------

## About

[![Github: Repo](https://img.shields.io/badge/GitHub-Repo-slategray?style=flat&logo=github&logoColor=black)](https://github.com/pgsty/extension)
[![Author: RuohangFeng](https://img.shields.io/badge/Author-Ruohang_Feng-steelblue?style=flat)](https://vonng.com/)
[![About: @Vonng](https://img.shields.io/badge/%40Vonng-steelblue?style=flat)](https://vonng.com/en/)
[![Mail: rh@vonng.com](https://img.shields.io/badge/rh%40vonng.com-steelblue?style=flat)](mailto:rh@vonng.com)
[![Copyright: 2018-2024 rh@Vonng.com](https://img.shields.io/badge/Copyright-2018--2024_(rh%40vonng.com)-red?logo=c&color=steelblue)](https://github.com/Vonng)
[![License: Apache-2.0](https://img.shields.io/badge/License-Apache2.0-steelblue?style=flat&logo=opensourceinitiative&logoColor=green)](https://pigsty.io/docs/about/license/)