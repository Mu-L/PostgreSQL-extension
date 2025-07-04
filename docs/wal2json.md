# wal2json


> [wal2json](https://github.com/eulerto/wal2json): Changing data capture in JSON format
>
> https://github.com/eulerto/wal2json





[ETL](/etl) extensions: [`pglogical`](/pglogical), [`pglogical_origin`](/pglogical_origin), [`pglogical_ticker`](/pglogical_ticker), [`pgl_ddl_deploy`](/pgl_ddl_deploy), [`pg_failover_slots`](/pg_failover_slots), [`db_migrator`](/db_migrator), [`pgactive`](/pgactive), [`wal2json`](/wal2json), [`wal2mongo`](/wal2mongo), [`decoderbufs`](/decoderbufs), [`decoder_raw`](/decoder_raw), [`mimeo`](/mimeo), [`repmgr`](/repmgr), [`pg_fact_loader`](/pg_fact_loader), [`pg_bulkload`](/pg_bulkload), [`test_decoding`](/test_decoding), [`pgoutput`](/pgoutput)


-------
## Extension


| Extension | Version | License | RPM | DEB | PL |
|-----------|:-------:|:-------:|:---:|:---:|:--:|
| [wal2json](https://github.com/eulerto/wal2json) | 2.6 | **<span class="tcblue">BSD-3</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tccyan">PGDG</span>** | `C` |



| `Bin` | `LOAD` | `DYLIB` | `DDL` | `TRUST` | `RELOC` |
|:-----:|:------:|:-------:|:-----:|:-------:|:-------:|
|  |  | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcwarn">✘</span> |  |



| Alias | Tags | Schemas | Requires | Required by |
|-------|------|---------|----------|-------------|
| [wal2json](/wal2json) |  |  |  |  |



| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `el9` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `d12` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `u22` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `u24` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |





-----------


## Packages


| OS | Version | License | REPO | Package Pattern | 17 | 16 | 15 | 14 | 13 | Dependency |
|:--:|---------|:-------:|:----:|-----------------|:--:|:--:|:--:|:--:|:--:|------------|
| [RPM](/rpm) | 2.6 | **<span class="tcblue">BSD-3</span>** | **<span class="tccyan">PGDG</span>** | `wal2json_$v*` | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** |  |
| [DEB](/deb) | 2.6 | **<span class="tcblue">BSD-3</span>** | **<span class="tccyan">PGDG</span>** | `postgresql-$v-wal2json` | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** |  |



Install `wal2json` via the [`pig`](https://github.com/pgsty/pig) cli tool:

```bash
pig ext add wal2json
```


Install `wal2json` via [Pigsty](https://pigsty.io/docs/pgext/usage/install/) playbook:

```bash
./pgsql.yml -t pg_extension -e '{"pg_extensions": ["wal2json"]}'
```


Install `wal2json` [RPM](/rpm) from the **<span class="tccyan">PGDG</span>** **YUM** repo:

```bash
dnf install wal2json_17*;
dnf install wal2json_16*;
dnf install wal2json_15*;
dnf install wal2json_14*;
dnf install wal2json_13*;
```


Install `wal2json` [DEB](/deb) from the **<span class="tccyan">PGDG</span>** **APT** repo:

```bash
apt install postgresql-17-wal2json;
apt install postgresql-16-wal2json;
apt install postgresql-15-wal2json;
apt install postgresql-14-wal2json;
apt install postgresql-13-wal2json;
```




| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | `wal2json_17*` | `wal2json_16*` | `wal2json_15*` | `wal2json_14*` | `wal2json_13*` |
| `el9` | `wal2json_17*` | `wal2json_16*` | `wal2json_15*` | `wal2json_14*` | `wal2json_13*` |
| `d12` | `postgresql-17-wal2json` | `postgresql-16-wal2json` | `postgresql-15-wal2json` | `postgresql-14-wal2json` | `postgresql-13-wal2json` |
| `u22` | `postgresql-17-wal2json` | `postgresql-16-wal2json` | `postgresql-15-wal2json` | `postgresql-14-wal2json` | `postgresql-13-wal2json` |
| `u24` | `postgresql-17-wal2json` | `postgresql-16-wal2json` | `postgresql-15-wal2json` | `postgresql-14-wal2json` | `postgresql-13-wal2json` |





