# log_fdw


> [log_fdw](https://github.com/aws/postgresql-logfdw): foreign-data wrapper for Postgres log file access
>
> https://github.com/aws/postgresql-logfdw





[FDW](/fdw) extensions: [`wrappers`](/wrappers), [`multicorn`](/multicorn), [`odbc_fdw`](/odbc_fdw), [`jdbc_fdw`](/jdbc_fdw), [`pgspider_ext`](/pgspider_ext), [`mysql_fdw`](/mysql_fdw), [`oracle_fdw`](/oracle_fdw), [`tds_fdw`](/tds_fdw), [`db2_fdw`](/db2_fdw), [`sqlite_fdw`](/sqlite_fdw), [`pgbouncer_fdw`](/pgbouncer_fdw), [`mongo_fdw`](/mongo_fdw), [`redis_fdw`](/redis_fdw), [`redis`](/redis), [`kafka_fdw`](/kafka_fdw), [`hdfs_fdw`](/hdfs_fdw), [`firebird_fdw`](/firebird_fdw), [`aws_s3`](/aws_s3), [`log_fdw`](/log_fdw), [`dblink`](/dblink), [`file_fdw`](/file_fdw), [`postgres_fdw`](/postgres_fdw)


-------
## Extension


| Extension | Version | License | RPM | DEB | PL |
|-----------|:-------:|:-------:|:---:|:---:|:--:|
| [log_fdw](https://github.com/aws/postgresql-logfdw) | 1.4 | **<span class="tccyan">Apache-2</span>** | **<span class="tcwarn">PIGSTY</span>** | **<span class="tcwarn">PIGSTY</span>** | `C` |



| `Bin` | `LOAD` | `DYLIB` | `DDL` | `TRUST` | `RELOC` |
|:-----:|:------:|:-------:|:-----:|:-------:|:-------:|
|  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |  |  |



| Alias | Tags | Schemas | Requires | Required by |
|-------|------|---------|----------|-------------|
| [log_fdw](/log_fdw) |  |  |  |  |



| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcred">✘</span> |
| `el9` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcred">✘</span> |
| `d12` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcred">✘</span> |
| `u22` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcred">✘</span> |
| `u24` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcred">✘</span> |





```sql
CREATE EXTENSION log_fdw;
```

-----------


## Packages


| OS | Version | License | REPO | Package Pattern | 17 | 16 | 15 | 14 | 13 | Dependency |
|:--:|---------|:-------:|:----:|-----------------|:--:|:--:|:--:|:--:|:--:|------------|
| [RPM](/rpm) | 1.4 | **<span class="tccyan">Apache-2</span>** | **<span class="tcwarn">PIGSTY</span>** | `log_fdw_$v*` | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** |  |  |
| [DEB](/deb) | 1.4 | **<span class="tccyan">Apache-2</span>** | **<span class="tcwarn">PIGSTY</span>** | `postgresql-$v-log-fdw` | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** |  |  |



Install `log_fdw` via the [`pig`](https://github.com/pgsty/pig) cli tool:

```bash
pig ext add log_fdw
```


Install `log_fdw` via [Pigsty](https://pigsty.io/docs/pgext/usage/install/) playbook:

```bash
./pgsql.yml -t pg_extension -e '{"pg_extensions": ["log_fdw"]}'
```


Install `log_fdw` [RPM](/rpm) from the **<span class="tcwarn">PIGSTY</span>** **YUM** repo:

```bash
dnf install log_fdw_17*;
dnf install log_fdw_16*;
dnf install log_fdw_15*;
dnf install log_fdw_14*;
```


Install `log_fdw` [DEB](/deb) from the **<span class="tcwarn">PIGSTY</span>** **APT** repo:

```bash
apt install postgresql-17-log-fdw;
apt install postgresql-16-log-fdw;
apt install postgresql-15-log-fdw;
apt install postgresql-14-log-fdw;
```




| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | `log_fdw_17*` | `log_fdw_16*` | `log_fdw_15*` | `log_fdw_14*` | <span class="tcred">✘</span> |
| `el9` | `log_fdw_17*` | `log_fdw_16*` | `log_fdw_15*` | `log_fdw_14*` | <span class="tcred">✘</span> |
| `d12` | `postgresql-17-log-fdw` | `postgresql-16-log-fdw` | `postgresql-15-log-fdw` | `postgresql-14-log-fdw` | <span class="tcred">✘</span> |
| `u22` | `postgresql-17-log-fdw` | `postgresql-16-log-fdw` | `postgresql-15-log-fdw` | `postgresql-14-log-fdw` | <span class="tcred">✘</span> |
| `u24` | `postgresql-17-log-fdw` | `postgresql-16-log-fdw` | `postgresql-15-log-fdw` | `postgresql-14-log-fdw` | <span class="tcred">✘</span> |





