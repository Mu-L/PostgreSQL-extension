# hashlib


> [pg_hashlib](https://github.com/markokr/pghashlib): Stable hash functions for Postgres
>
> https://github.com/markokr/pghashlib





[UTIL](/util) extensions: [`gzip`](/gzip), [`bzip`](/bzip), [`zstd`](/zstd), [`http`](/http), [`pg_net`](/pg_net), [`pg_curl`](/pg_curl), [`pgjq`](/pgjq), [`pgjwt`](/pgjwt), [`pg_smtp_client`](/pg_smtp_client), [`pg_html5_email_address`](/pg_html5_email_address), [`url_encode`](/url_encode), [`pgsql_tweaks`](/pgsql_tweaks), [`pg_extra_time`](/pg_extra_time), [`pgpcre`](/pgpcre), [`icu_ext`](/icu_ext), [`pgqr`](/pgqr), [`pg_protobuf`](/pg_protobuf), [`envvar`](/envvar), [`floatfile`](/floatfile), [`pg_render`](/pg_render), [`pg_readme`](/pg_readme), [`pg_readme_test_extension`](/pg_readme_test_extension), [`ddl_historization`](/ddl_historization), [`data_historization`](/data_historization), [`schedoc`](/schedoc), [`hashlib`](/hashlib), [`xxhash`](/xxhash), [`shacrypt`](/shacrypt), [`cryptint`](/cryptint), [`pguecc`](/pguecc), [`sparql`](/sparql)


-------
## Extension


| Extension | Version | License | RPM | DEB | PL |
|-----------|:-------:|:-------:|:---:|:---:|:--:|
| [hashlib](https://github.com/markokr/pghashlib) | 1.1 | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcwarn">PIGSTY</span>** | **<span class="tcwarn">PIGSTY</span>** | `C` |



| `Bin` | `LOAD` | `DYLIB` | `DDL` | `TRUST` | `RELOC` |
|:-----:|:------:|:-------:|:-----:|:-------:|:-------:|
|  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |



| Alias | Tags | Schemas | Requires | Required by |
|-------|------|---------|----------|-------------|
| [pg_hashlib](/hashlib) |  |  |  |  |



| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `el9` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `d12` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `u22` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `u24` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |





```sql
CREATE EXTENSION hashlib;
```

-----------


## Packages


| OS | Version | License | REPO | Package Pattern | 17 | 16 | 15 | 14 | 13 | Dependency |
|:--:|---------|:-------:|:----:|-----------------|:--:|:--:|:--:|:--:|:--:|------------|
| [RPM](/rpm) | 1.1 | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcwarn">PIGSTY</span>** | `pg_hashlib_$v` | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** |  |
| [DEB](/deb) | 1.1 | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcwarn">PIGSTY</span>** | `postgresql-$v-pg-hashlib` | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** |  |



Install `hashlib` via the [`pig`](https://github.com/pgsty/pig) cli tool:

```bash
pig ext add hashlib
```


Install `pg_hashlib` via [Pigsty](https://pigsty.io/docs/pgext/usage/install/) playbook:

```bash
./pgsql.yml -t pg_extension -e '{"pg_extensions": ["pg_hashlib"]}'
```


Install `pg_hashlib` [RPM](/rpm) from the **<span class="tcwarn">PIGSTY</span>** **YUM** repo:

```bash
dnf install pg_hashlib_17;
dnf install pg_hashlib_16;
dnf install pg_hashlib_15;
dnf install pg_hashlib_14;
dnf install pg_hashlib_13;
```


Install `pg_hashlib` [DEB](/deb) from the **<span class="tcwarn">PIGSTY</span>** **APT** repo:

```bash
apt install postgresql-17-pg-hashlib;
apt install postgresql-16-pg-hashlib;
apt install postgresql-15-pg-hashlib;
apt install postgresql-14-pg-hashlib;
apt install postgresql-13-pg-hashlib;
```




| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | `pg_hashlib_17` | `pg_hashlib_16` | `pg_hashlib_15` | `pg_hashlib_14` | `pg_hashlib_13` |
| `el9` | `pg_hashlib_17` | `pg_hashlib_16` | `pg_hashlib_15` | `pg_hashlib_14` | `pg_hashlib_13` |
| `d12` | `postgresql-17-pg-hashlib` | `postgresql-16-pg-hashlib` | `postgresql-15-pg-hashlib` | `postgresql-14-pg-hashlib` | `postgresql-13-pg-hashlib` |
| `u22` | `postgresql-17-pg-hashlib` | `postgresql-16-pg-hashlib` | `postgresql-15-pg-hashlib` | `postgresql-14-pg-hashlib` | `postgresql-13-pg-hashlib` |
| `u24` | `postgresql-17-pg-hashlib` | `postgresql-16-pg-hashlib` | `postgresql-15-pg-hashlib` | `postgresql-14-pg-hashlib` | `postgresql-13-pg-hashlib` |





