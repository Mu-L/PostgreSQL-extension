# pg_idkit


> [pg_idkit](https://github.com/VADOSWARE/pg_idkit): multi-tool for generating new/niche universally unique identifiers (ex. UUIDv6, ULID, KSUID)
>
> https://github.com/VADOSWARE/pg_idkit





[FUNC](/func) extensions: [`pg_idkit`](/pg_idkit), [`pgx_ulid`](/pgx_ulid), [`pg_uuidv7`](/pg_uuidv7), [`permuteseq`](/permuteseq), [`pg_hashids`](/pg_hashids), [`sequential_uuids`](/sequential_uuids), [`topn`](/topn), [`quantile`](/quantile), [`lower_quantile`](/lower_quantile), [`count_distinct`](/count_distinct), [`omnisketch`](/omnisketch), [`ddsketch`](/ddsketch), [`vasco`](/vasco), [`xicor`](/xicor), [`tdigest`](/tdigest), [`first_last_agg`](/first_last_agg), [`extra_window_functions`](/extra_window_functions), [`floatvec`](/floatvec), [`aggs_for_vecs`](/aggs_for_vecs), [`aggs_for_arrays`](/aggs_for_arrays), [`arraymath`](/arraymath), [`pg_math`](/pg_math), [`random`](/random), [`base36`](/base36), [`base62`](/base62), [`pg_base58`](/pg_base58), [`financial`](/financial), [`convert`](/convert), [`refint`](/refint), [`autoinc`](/autoinc), [`insert_username`](/insert_username), [`moddatetime`](/moddatetime), [`tsm_system_time`](/tsm_system_time), [`dict_xsyn`](/dict_xsyn), [`tsm_system_rows`](/tsm_system_rows), [`tcn`](/tcn), [`uuid-ossp`](/uuid-ossp), [`btree_gist`](/btree_gist), [`btree_gin`](/btree_gin), [`intarray`](/intarray), [`intagg`](/intagg), [`dict_int`](/dict_int), [`unaccent`](/unaccent)


-------
## Extension


| Extension | Version | License | RPM | DEB | PL |
|-----------|:-------:|:-------:|:---:|:---:|:--:|
| [pg_idkit](https://github.com/VADOSWARE/pg_idkit) | 0.3.0 | **<span class="tccyan">Apache-2</span>** | **<span class="tcwarn">PIGSTY</span>** | **<span class="tcwarn">PIGSTY</span>** | `Rust` |



| `Bin` | `LOAD` | `DYLIB` | `DDL` | `TRUST` | `RELOC` |
|:-----:|:------:|:-------:|:-----:|:-------:|:-------:|
|  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcwarn">✘</span> |



| Alias | Tags | Schemas | Requires | Required by |
|-------|------|---------|----------|-------------|
| [pg_idkit](/pg_idkit) | `pgrx` |  |  |  |



| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `el9` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `d12` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `u22` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `u24` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |





```sql
CREATE EXTENSION pg_idkit;
```
> **Comment**: pgrx=0.14.1
-----------


## Packages


| OS | Version | License | REPO | Package Pattern | 17 | 16 | 15 | 14 | 13 | Dependency |
|:--:|---------|:-------:|:----:|-----------------|:--:|:--:|:--:|:--:|:--:|------------|
| [RPM](/rpm) | 0.3.0 | **<span class="tccyan">Apache-2</span>** | **<span class="tcwarn">PIGSTY</span>** | `pg_idkit_$v` | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** |  |
| [DEB](/deb) | 0.3.0 | **<span class="tccyan">Apache-2</span>** | **<span class="tcwarn">PIGSTY</span>** | `postgresql-$v-pg-idkit` | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** | **<span class="tcwarn">✔</span>** |  |



Install `pg_idkit` via the [`pig`](https://github.com/pgsty/pig) cli tool:

```bash
pig ext add pg_idkit
```


Install `pg_idkit` via [Pigsty](https://pigsty.io/docs/pgext/usage/install/) playbook:

```bash
./pgsql.yml -t pg_extension -e '{"pg_extensions": ["pg_idkit"]}'
```


Install `pg_idkit` [RPM](/rpm) from the **<span class="tcwarn">PIGSTY</span>** **YUM** repo:

```bash
dnf install pg_idkit_17;
dnf install pg_idkit_16;
dnf install pg_idkit_15;
dnf install pg_idkit_14;
dnf install pg_idkit_13;
```


Install `pg_idkit` [DEB](/deb) from the **<span class="tcwarn">PIGSTY</span>** **APT** repo:

```bash
apt install postgresql-17-pg-idkit;
apt install postgresql-16-pg-idkit;
apt install postgresql-15-pg-idkit;
apt install postgresql-14-pg-idkit;
apt install postgresql-13-pg-idkit;
```




| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | `pg_idkit_17` | `pg_idkit_16` | `pg_idkit_15` | `pg_idkit_14` | `pg_idkit_13` |
| `el9` | `pg_idkit_17` | `pg_idkit_16` | `pg_idkit_15` | `pg_idkit_14` | `pg_idkit_13` |
| `d12` | `postgresql-17-pg-idkit` | `postgresql-16-pg-idkit` | `postgresql-15-pg-idkit` | `postgresql-14-pg-idkit` | `postgresql-13-pg-idkit` |
| `u22` | `postgresql-17-pg-idkit` | `postgresql-16-pg-idkit` | `postgresql-15-pg-idkit` | `postgresql-14-pg-idkit` | `postgresql-13-pg-idkit` |
| `u24` | `postgresql-17-pg-idkit` | `postgresql-16-pg-idkit` | `postgresql-15-pg-idkit` | `postgresql-14-pg-idkit` | `postgresql-13-pg-idkit` |





