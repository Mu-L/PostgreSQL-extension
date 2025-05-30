# tdigest


> [tdigest](https://github.com/tvondra/tdigest): Provides tdigest aggregate function.
>
> https://github.com/tvondra/tdigest





[FUNC](/func) extensions: [`pg_idkit`](/pg_idkit), [`pgx_ulid`](/pgx_ulid), [`pg_uuidv7`](/pg_uuidv7), [`permuteseq`](/permuteseq), [`pg_hashids`](/pg_hashids), [`sequential_uuids`](/sequential_uuids), [`topn`](/topn), [`quantile`](/quantile), [`lower_quantile`](/lower_quantile), [`count_distinct`](/count_distinct), [`omnisketch`](/omnisketch), [`ddsketch`](/ddsketch), [`vasco`](/vasco), [`xicor`](/xicor), [`tdigest`](/tdigest), [`first_last_agg`](/first_last_agg), [`extra_window_functions`](/extra_window_functions), [`floatvec`](/floatvec), [`aggs_for_vecs`](/aggs_for_vecs), [`aggs_for_arrays`](/aggs_for_arrays), [`arraymath`](/arraymath), [`pg_math`](/pg_math), [`random`](/random), [`base36`](/base36), [`base62`](/base62), [`pg_base58`](/pg_base58), [`financial`](/financial), [`convert`](/convert), [`refint`](/refint), [`autoinc`](/autoinc), [`insert_username`](/insert_username), [`moddatetime`](/moddatetime), [`tsm_system_time`](/tsm_system_time), [`dict_xsyn`](/dict_xsyn), [`tsm_system_rows`](/tsm_system_rows), [`tcn`](/tcn), [`uuid-ossp`](/uuid-ossp), [`btree_gist`](/btree_gist), [`btree_gin`](/btree_gin), [`intarray`](/intarray), [`intagg`](/intagg), [`dict_int`](/dict_int), [`unaccent`](/unaccent)


-------
## Extension


| Extension | Version | License | RPM | DEB | PL |
|-----------|:-------:|:-------:|:---:|:---:|:--:|
| [tdigest](https://github.com/tvondra/tdigest) | 1.4.3 | **<span class="tccyan">Apache-2</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tccyan">PGDG</span>** | `C` |



| `Bin` | `LOAD` | `DYLIB` | `DDL` | `TRUST` | `RELOC` |
|:-----:|:------:|:-------:|:-----:|:-------:|:-------:|
|  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |



| Alias | Tags | Schemas | Requires | Required by |
|-------|------|---------|----------|-------------|
| [tdigest](/tdigest) |  |  |  |  |



| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `el9` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `d12` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `u22` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |
| `u24` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |





```sql
CREATE EXTENSION tdigest;
```

-----------


## Packages


| OS | Version | License | REPO | Package Pattern | 17 | 16 | 15 | 14 | 13 | Dependency |
|:--:|---------|:-------:|:----:|-----------------|:--:|:--:|:--:|:--:|:--:|------------|
| [RPM](/rpm) | 1.4.2 | **<span class="tccyan">Apache-2</span>** | **<span class="tccyan">PGDG</span>** | `tdigest_$v*` | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** |  |
| [DEB](/deb) | 1.4.3 | **<span class="tccyan">Apache-2</span>** | **<span class="tccyan">PGDG</span>** | `postgresql-$v-tdigest` | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** | **<span class="tccyan">✔</span>** |  |



Install `tdigest` via the [`pig`](https://github.com/pgsty/pig) cli tool:

```bash
pig ext add tdigest
```


Install `tdigest` via [Pigsty](https://pigsty.io/docs/pgext/usage/install/) playbook:

```bash
./pgsql.yml -t pg_extension -e '{"pg_extensions": ["tdigest"]}'
```


Install `tdigest` [RPM](/rpm) from the **<span class="tccyan">PGDG</span>** **YUM** repo:

```bash
dnf install tdigest_17*;
dnf install tdigest_16*;
dnf install tdigest_15*;
dnf install tdigest_14*;
dnf install tdigest_13*;
```


Install `tdigest` [DEB](/deb) from the **<span class="tccyan">PGDG</span>** **APT** repo:

```bash
apt install postgresql-17-tdigest;
apt install postgresql-16-tdigest;
apt install postgresql-15-tdigest;
apt install postgresql-14-tdigest;
apt install postgresql-13-tdigest;
```




| Distro / Ver | PG17 | PG16 | PG15 | PG14 | PG13 |
|:------------:|:----:|:----:|:----:|:----:|:----:|
| `el8` | `tdigest_17*` | `tdigest_16*` | `tdigest_15*` | `tdigest_14*` | `tdigest_13*` |
| `el9` | `tdigest_17*` | `tdigest_16*` | `tdigest_15*` | `tdigest_14*` | `tdigest_13*` |
| `d12` | `postgresql-17-tdigest` | `postgresql-16-tdigest` | `postgresql-15-tdigest` | `postgresql-14-tdigest` | `postgresql-13-tdigest` |
| `u22` | `postgresql-17-tdigest` | `postgresql-16-tdigest` | `postgresql-15-tdigest` | `postgresql-14-tdigest` | `postgresql-13-tdigest` |
| `u24` | `postgresql-17-tdigest` | `postgresql-16-tdigest` | `postgresql-15-tdigest` | `postgresql-14-tdigest` | `postgresql-13-tdigest` |





