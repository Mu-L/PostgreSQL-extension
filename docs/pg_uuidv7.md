# pg_uuidv7


> [pg_uuidv7](https://github.com/fboulnois/pg_uuidv7): Create UUIDv7 values in postgres
>
> https://github.com/fboulnois/pg_uuidv7





[FUNC](/func) extensions: [`pg_idkit`](/pg_idkit), [`pgx_ulid`](/pgx_ulid), [`pg_uuidv7`](/pg_uuidv7), [`permuteseq`](/permuteseq), [`pg_hashids`](/pg_hashids), [`sequential_uuids`](/sequential_uuids), [`topn`](/topn), [`quantile`](/quantile), [`lower_quantile`](/lower_quantile), [`count_distinct`](/count_distinct), [`omnisketch`](/omnisketch), [`ddsketch`](/ddsketch), [`vasco`](/vasco), [`xicor`](/xicor), [`tdigest`](/tdigest), [`first_last_agg`](/first_last_agg), [`extra_window_functions`](/extra_window_functions), [`floatvec`](/floatvec), [`aggs_for_vecs`](/aggs_for_vecs), [`aggs_for_arrays`](/aggs_for_arrays), [`arraymath`](/arraymath), [`pg_math`](/pg_math), [`random`](/random), [`base36`](/base36), [`base62`](/base62), [`pg_base58`](/pg_base58), [`financial`](/financial), [`convert`](/convert), [`refint`](/refint), [`autoinc`](/autoinc), [`insert_username`](/insert_username), [`moddatetime`](/moddatetime), [`tsm_system_time`](/tsm_system_time), [`dict_xsyn`](/dict_xsyn), [`tsm_system_rows`](/tsm_system_rows), [`tcn`](/tcn), [`uuid-ossp`](/uuid-ossp), [`btree_gist`](/btree_gist), [`btree_gin`](/btree_gin), [`intarray`](/intarray), [`intagg`](/intagg), [`dict_int`](/dict_int), [`unaccent`](/unaccent)


-------
## Extension


| Extension | Version | License | RPM | DEB | PL |
|-----------|:-------:|:-------:|:---:|:---:|:--:|
| [pg_uuidv7](https://github.com/fboulnois/pg_uuidv7) | 1.6.0 | **<span class="tccyan">MPLv2</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tcwarn">PIGSTY</span>** | `C` |



| `Bin` | `LOAD` | `DYLIB` | `DDL` | `TRUST` | `RELOC` |
|:-----:|:------:|:-------:|:-----:|:-------:|:-------:|
|  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |



| Alias | Tags | Schemas | Requires | Required by |
|-------|------|---------|----------|-------------|
| [pg_uuidv7](/pg_uuidv7) |  |  |  |  |



| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `el9` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `d12` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `u22` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `u24` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |





```sql
CREATE EXTENSION pg_uuidv7;
```

-----------


## Packages


| OS | Version | License | REPO | Package Pattern | 17 | 16 | 15 | 14 | 13 | Dependency |
|:--:|---------|:-------:|:----:|-----------------|:--:|:--:|:--:|:--:|:--:|------------|
| [RPM](/rpm) | 1.6.0 | **<span class="tccyan">MPLv2</span>** | **<span class="tccyan">PGDG</span>** | `pg_uuidv7_$v*` | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** |  |
| [DEB](/deb) | 1.6.0 | **<span class="tccyan">MPLv2</span>** | **<span class="tcwarn">PIGSTY</span>** | `postgresql-$v-pg-uuidv7` | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** |  |



Install `pg_uuidv7` via the [`pig`](https://github.com/pgsty/pig) cli tool:

```bash
pig ext add pg_uuidv7
```


Install `pg_uuidv7` via [Pigsty](https://pigsty.io/docs/pgext/usage/install/) playbook:

```bash
./pgsql.yml -t pg_extension -e '{"pg_extensions": ["pg_uuidv7"]}'
```


Install `pg_uuidv7` [RPM](/rpm) from the **<span class="tccyan">PGDG</span>** **YUM** repo:

```bash
dnf install pg_uuidv7_17*;
dnf install pg_uuidv7_16*;
dnf install pg_uuidv7_15*;
dnf install pg_uuidv7_14*;
dnf install pg_uuidv7_13*;
```


Install `pg_uuidv7` [DEB](/deb) from the **<span class="tcwarn">PIGSTY</span>** **APT** repo:

```bash
apt install postgresql-17-pg-uuidv7;
apt install postgresql-16-pg-uuidv7;
apt install postgresql-15-pg-uuidv7;
apt install postgresql-14-pg-uuidv7;
apt install postgresql-13-pg-uuidv7;
```




| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | `pg_uuidv7_17*` | `pg_uuidv7_16*` | `pg_uuidv7_15*` | `pg_uuidv7_14*` | `pg_uuidv7_13*` |
| `el9` | `pg_uuidv7_17*` | `pg_uuidv7_16*` | `pg_uuidv7_15*` | `pg_uuidv7_14*` | `pg_uuidv7_13*` |
| `d12` | `postgresql-17-pg-uuidv7` | `postgresql-16-pg-uuidv7` | `postgresql-15-pg-uuidv7` | `postgresql-14-pg-uuidv7` | `postgresql-13-pg-uuidv7` |
| `u22` | `postgresql-17-pg-uuidv7` | `postgresql-16-pg-uuidv7` | `postgresql-15-pg-uuidv7` | `postgresql-14-pg-uuidv7` | `postgresql-13-pg-uuidv7` |
| `u24` | `postgresql-17-pg-uuidv7` | `postgresql-16-pg-uuidv7` | `postgresql-15-pg-uuidv7` | `postgresql-14-pg-uuidv7` | `postgresql-13-pg-uuidv7` |





