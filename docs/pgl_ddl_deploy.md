# pgl_ddl_deploy


> [pgl_ddl_deploy](https://github.com/enova/pgl_ddl_deploy): automated ddl deployment using pglogical
>
> https://github.com/enova/pgl_ddl_deploy





[ETL](/etl) extensions: [`pglogical`](/pglogical), [`pglogical_origin`](/pglogical_origin), [`pglogical_ticker`](/pglogical_ticker), [`pgl_ddl_deploy`](/pgl_ddl_deploy), [`pg_failover_slots`](/pg_failover_slots), [`db_migrator`](/db_migrator), [`pgactive`](/pgactive), [`wal2json`](/wal2json), [`wal2mongo`](/wal2mongo), [`decoderbufs`](/decoderbufs), [`decoder_raw`](/decoder_raw), [`mimeo`](/mimeo), [`repmgr`](/repmgr), [`pg_fact_loader`](/pg_fact_loader), [`pg_bulkload`](/pg_bulkload), [`test_decoding`](/test_decoding), [`pgoutput`](/pgoutput)


-------
## Extension


| Extension | Version | License | RPM | DEB | PL |
|-----------|:-------:|:-------:|:---:|:---:|:--:|
| [pgl_ddl_deploy](https://github.com/enova/pgl_ddl_deploy) | 2.2.1 | **<span class="tcblue">MIT</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tccyan">PGDG</span>** | `C` |



| `Bin` | `LOAD` | `DYLIB` | `DDL` | `TRUST` | `RELOC` |
|:-----:|:------:|:-------:|:-----:|:-------:|:-------:|
|  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |  |



| Alias | Tags | Schemas | Requires | Required by |
|-------|------|---------|----------|-------------|
| [pgl_ddl_deploy](/pgl_ddl_deploy) |  | `pgl_ddl_deploy` | [`pglogical`](pglogical) |  |



| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `el9` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `d12` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `u22` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `u24` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |





```sql
CREATE EXTENSION pgl_ddl_deploy CASCADE;
```

-----------


## Packages


| OS | Version | License | REPO | Package Pattern | 17 | 16 | 15 | 14 | 13 | Dependency |
|:--:|---------|:-------:|:----:|-----------------|:--:|:--:|:--:|:--:|:--:|------------|
| [RPM](/rpm) | 2.2.1 | **<span class="tcblue">MIT</span>** | **<span class="tccyan">PGDG</span>** | `pgl_ddl_deploy_$v*` | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | `pglogical_$v` |
| [DEB](/deb) | 2.2.1 | **<span class="tcblue">MIT</span>** | **<span class="tccyan">PGDG</span>** | `postgresql-$v-pgl-ddl-deploy` | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | `postgresql-$v-pglogical` |



Install `pgl_ddl_deploy` via the [`pig`](https://github.com/pgsty/pig) cli tool:

```bash
pig ext add pgl_ddl_deploy
```


Install `pgl_ddl_deploy` via [Pigsty](https://pigsty.io/docs/pgext/usage/install/) playbook:

```bash
./pgsql.yml -t pg_extension -e '{"pg_extensions": ["pgl_ddl_deploy"]}'
```


Install `pgl_ddl_deploy` [RPM](/rpm) from the **<span class="tccyan">PGDG</span>** **YUM** repo:

```bash
dnf install pgl_ddl_deploy_17*;
dnf install pgl_ddl_deploy_16*;
dnf install pgl_ddl_deploy_15*;
dnf install pgl_ddl_deploy_14*;
dnf install pgl_ddl_deploy_13*;
```


Install `pgl_ddl_deploy` [DEB](/deb) from the **<span class="tccyan">PGDG</span>** **APT** repo:

```bash
apt install postgresql-17-pgl-ddl-deploy;
apt install postgresql-16-pgl-ddl-deploy;
apt install postgresql-15-pgl-ddl-deploy;
apt install postgresql-14-pgl-ddl-deploy;
apt install postgresql-13-pgl-ddl-deploy;
```




| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | `pgl_ddl_deploy_17*` | `pgl_ddl_deploy_16*` | `pgl_ddl_deploy_15*` | `pgl_ddl_deploy_14*` | `pgl_ddl_deploy_13*` |
| `el9` | `pgl_ddl_deploy_17*` | `pgl_ddl_deploy_16*` | `pgl_ddl_deploy_15*` | `pgl_ddl_deploy_14*` | `pgl_ddl_deploy_13*` |
| `d12` | `postgresql-17-pgl-ddl-deploy` | `postgresql-16-pgl-ddl-deploy` | `postgresql-15-pgl-ddl-deploy` | `postgresql-14-pgl-ddl-deploy` | `postgresql-13-pgl-ddl-deploy` |
| `u22` | `postgresql-17-pgl-ddl-deploy` | `postgresql-16-pgl-ddl-deploy` | `postgresql-15-pgl-ddl-deploy` | `postgresql-14-pgl-ddl-deploy` | `postgresql-13-pgl-ddl-deploy` |
| `u24` | `postgresql-17-pgl-ddl-deploy` | `postgresql-16-pgl-ddl-deploy` | `postgresql-15-pgl-ddl-deploy` | `postgresql-14-pgl-ddl-deploy` | `postgresql-13-pgl-ddl-deploy` |





