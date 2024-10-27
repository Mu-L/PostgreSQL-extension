# pg_wait_sampling


> [pg_wait_sampling](/https://github.com/postgrespro/pg_wait_sampling): sampling based statistics of wait events


-------

## Extension


| ID | Extension | Version | License | RPM | DEB | `LOAD` | `DYLIB` | `DDL` | `TRUST` | `RELOC` | Requires |
|:--:|-----------|:-------:|:-------:|:---:|:---:|:------:|:-------:|:-----:|:-------:|:-------:|----------|
| 6070 | [pg_wait_sampling](https://github.com/postgrespro/pg_wait_sampling) | 1.1 | **<span class="tcblue">PostgreSQL</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tccyan">PGDG</span>** | <span class="tcred">❗</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |  |




```bash
shared_preload_libraries = 'pg_wait_sampling'; # add this extension to postgresql.conf
```


```sql
CREATE EXTENSION pg_wait_sampling;
```


-----------


## Packages


| OS | Version | License | RPM | RPM Package | 17 | 16 | 15 | 14 | 13 | 12 | Dependency |
|:--:|---------|:-------:|:---:|-------------|:--:|:--:|:--:|:--:|:--:|:--:|------------|
| [RPM](/rpm) | 1.1 | **<span class="tcblue">PostgreSQL</span>** | **<span class="tccyan">PGDG</span>** | `pg_wait_sampling_$v*` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |  |
| [DEB](/deb) | 1.1 | **<span class="tcblue">PostgreSQL</span>** | **<span class="tccyan">PGDG</span>** | `postgresql-$v-pg-wait-sampling` | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |  |



Install `pg_wait_sampling` [RPM](/rpm) from the **<span class="tccyan">PGDG</span>** **YUM** repo:

```bash
dnf install pg_wait_sampling_17*;
dnf install pg_wait_sampling_16*;
dnf install pg_wait_sampling_15*;
dnf install pg_wait_sampling_14*;
dnf install pg_wait_sampling_13*;
dnf install pg_wait_sampling_12*;
```


Install `pg_wait_sampling` [DEB](/deb) from the **<span class="tccyan">PGDG</span>** **APT** repo:

```bash
apt install postgresql-17-pg-wait-sampling;
apt install postgresql-16-pg-wait-sampling;
apt install postgresql-15-pg-wait-sampling;
apt install postgresql-14-pg-wait-sampling;
apt install postgresql-13-pg-wait-sampling;
apt install postgresql-12-pg-wait-sampling;
```


-----------


## Category: STAT


| ID | Extension | Version | Package | License | RPM | DEB | lang | Tags | Schemas | Requires | `LOAD` | `DYLIB` | `DDL` | `TRUST` | `RELOC` |
|:--:|-----------|:-------:|---------|:-------:|:---:|:---:|:----:|------|---------|----------|:------:|:-------:|:-----:|:-------:|:-------:|
| 6000 | [pg_profile](/stat/pg_profile) | 4.7 | [pg_profile](/stat/pg_profile) | **<span class="tcblue">BSD-2</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tcwarn">PIGSTY</span>** |  |  |  | [`dblink`](/fdw/dblink), [`plpgsql`](/lang/plpgsql) |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcwarn">✘</span> |
| 6010 | [pg_show_plans](/stat/pg_show_plans) | 2.1 | [pg_show_plans](/stat/pg_show_plans) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tccyan">PGDG</span>** |  |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |
| 6020 | [pg_stat_kcache](/stat/pg_stat_kcache) | 2.3.0 | [pg_stat_kcache](/stat/pg_stat_kcache) | **<span class="tcblue">BSD-3</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tccyan">PGDG</span>** |  |  |  | [`pg_stat_statements`](/stat/pg_stat_statements) | <span class="tcred">❗</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |
| 6030 | [pg_stat_monitor](/stat/pg_stat_monitor) | 2.1 | [pg_stat_monitor](/stat/pg_stat_monitor) | **<span class="tcblue">BSD-3</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tcwarn">PIGSTY</span>** |  |  |  |  | <span class="tcred">❗</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |
| 6040 | [pg_qualstats](/stat/pg_qualstats) | 2.1.1 | [pg_qualstats](/stat/pg_qualstats) | **<span class="tcblue">BSD-3</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tccyan">PGDG</span>** |  |  |  |  | <span class="tcred">❗</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcwarn">✘</span> |
| 6050 | [pg_store_plans](/stat/pg_store_plans) | 1.8 | [pg_store_plans](/stat/pg_store_plans) | **<span class="tcblue">BSD-3</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tcwarn">PIGSTY</span>** |  |  |  |  | <span class="tcred">❗</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |
| 6060 | [pg_track_settings](/stat/pg_track_settings) | 2.1.2 | [pg_track_settings](/stat/pg_track_settings) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tccyan">PGDG</span>** |  |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |
| 6070 | [pg_wait_sampling](/stat/pg_wait_sampling) | 1.1 | [pg_wait_sampling](/stat/pg_wait_sampling) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tccyan">PGDG</span>** |  |  |  |  | <span class="tcred">❗</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |
| 6080 | [system_stats](/stat/system_stats) | 3.0 | [system_stats](/stat/system_stats) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tcwarn">PIGSTY</span>** |  |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |
| 6090 | [meta](/stat/meta) | 0.4.0 | [pg_meta](/stat/meta) | **<span class="tcblue">BSD-2</span>** | **<span class="tcwarn">PIGSTY</span>** | **<span class="tcwarn">PIGSTY</span>** | SQL |  |  |  |  | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |  | <span class="tcblue">✔</span> |
| 6100 | [pgnodemx](/stat/pgnodemx) | 1.7 | [pgnodemx](/stat/pgnodemx) | **<span class="tccyan">Apache-2</span>** | **<span class="tcwarn">PIGSTY</span>** | **<span class="tcwarn">PIGSTY</span>** | C |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |
| 6120 | [pg_proctab](/stat/pg_proctab) | 0.0.10-compat | [pgnodemx](/stat/pg_proctab) | **<span class="tcblue">BSD-3</span>** | **<span class="tcwarn">PIGSTY</span>** | **<span class="tcwarn">PIGSTY</span>** |  |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |
| 6130 | [pg_sqlog](/stat/pg_sqlog) | 1.6 | [pg_sqlog](/stat/pg_sqlog) | **<span class="tcblue">BSD-3</span>** | **<span class="tcwarn">PIGSTY</span>** | **<span class="tcwarn">PIGSTY</span>** |  |  | `sqlog` | [`file_fdw`](/fdw/file_fdw) |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcwarn">✘</span> |
| 6140 | [bgw_replstatus](/stat/bgw_replstatus) | 1.0.6 | [bgw_replstatus](/stat/bgw_replstatus) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tccyan">PGDG</span>** | C |  |  |  | <span class="tcred">❗</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcwarn">✘</span> |  |
| 6150 | [pgmeminfo](/stat/pgmeminfo) | 1.0 | [pgmeminfo](/stat/pgmeminfo) | **<span class="tcblue">MIT</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tcwarn">PIGSTY</span>** |  |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcwarn">✘</span> |
| 6160 | [toastinfo](/stat/toastinfo) | 1 | [toastinfo](/stat/toastinfo) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcwarn">PIGSTY</span>** | **<span class="tcwarn">PIGSTY</span>** |  |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |
| 6170 | [explain_ui](/stat/explain_ui) | 0.0.1 | [pg_explain_ui](/stat/explain_ui) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcwarn">PIGSTY</span>** | **<span class="tcwarn">PIGSTY</span>** | Rust | `pgrx` |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |
| 6180 | [pg_relusage](/stat/pg_relusage) | 0.0.1 | [pg_relusage](/stat/pg_relusage) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcwarn">PIGSTY</span>** | **<span class="tcwarn">PIGSTY</span>** |  |  |  |  | <span class="tcred">❗</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcwarn">✘</span> | <span class="tcwarn">✘</span> |
| 6190 | [pg_mon](/stat/pg_mon) | 1.0 | [pg_mon](/stat/pg_mon) | **<span class="tcblue">MIT</span>** | **<span class="tcwarn">PIGSTY</span>** | **<span class="tcwarn">PIGSTY</span>** | C |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> |  |  |
| 6200 | [pg_statviz](/stat/pg_statviz) | 0.6 | [pg_statviz](/stat/pg_statviz) | **<span class="tcblue">BSD-3</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tccyan">PGDG</span>** | Python | `not-used` |  |  |  | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |  |
| 6210 | [pgexporter_ext](/stat/pgexporter_ext) | 0.2.3 | [pgexporter_ext](/stat/pgexporter_ext) | **<span class="tcblue">BSD-3</span>** | **<span class="tccyan">PGDG</span>** | PGDG | C | `not-used` |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |  |
| 6220 | [pg_top](/stat/pg_top) | 3.7.0 | [pg_top](/stat/pg_top) | **<span class="tcblue">BSD-3</span>** | **<span class="tccyan">PGDG</span>** | PGDG | C |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcwarn">✘</span> |  |
| 6230 | [pagevis](/stat/pagevis) | 0.1 | [pagevis](/stat/pagevis) | **<span class="tcblue">MIT</span>** | **<span class="tcwarn">PIGSTY</span>** | **<span class="tcwarn">PIGSTY</span>** | SQL |  |  |  |  | <span class="tcwarn">✘</span> | <span class="tcblue">✔</span> |  | <span class="tcblue">✔</span> |
| 6240 | [powa](/stat/powa) | 4.2.2 | [powa](/stat/powa) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tccyan">PGDG</span>** | **<span class="tccyan">PGDG</span>** |  |  | `public` | [`plpgsql`](/lang/plpgsql), [`pg_stat_statements`](/stat/pg_stat_statements), [`btree_gist`](/func/btree_gist) |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcwarn">✘</span> |
| 6900 | [pageinspect](/stat/pageinspect) | 1.12 | [pageinspect](/stat/pageinspect) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcblue">CONTRIB</span>** | **<span class="tcblue">CONTRIB</span>** | C |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |  |
| 6910 | [pgrowlocks](/stat/pgrowlocks) | 1.2 | [pgrowlocks](/stat/pgrowlocks) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcblue">CONTRIB</span>** | **<span class="tcblue">CONTRIB</span>** | C |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |  |
| 6920 | [sslinfo](/stat/sslinfo) | 1.2 | [sslinfo](/stat/sslinfo) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcblue">CONTRIB</span>** | **<span class="tcblue">CONTRIB</span>** | C |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |  |
| 6930 | [pg_buffercache](/stat/pg_buffercache) | 1.4 | [pg_buffercache](/stat/pg_buffercache) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcblue">CONTRIB</span>** | **<span class="tcblue">CONTRIB</span>** | C |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |  |
| 6940 | [pg_walinspect](/stat/pg_walinspect) | 1.1 | [pg_walinspect](/stat/pg_walinspect) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcblue">CONTRIB</span>** | **<span class="tcblue">CONTRIB</span>** | C |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |  |
| 6950 | [pg_freespacemap](/stat/pg_freespacemap) | 1.2 | [pg_freespacemap](/stat/pg_freespacemap) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcblue">CONTRIB</span>** | **<span class="tcblue">CONTRIB</span>** | C |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |  |
| 6960 | [pg_visibility](/stat/pg_visibility) | 1.2 | [pg_visibility](/stat/pg_visibility) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcblue">CONTRIB</span>** | **<span class="tcblue">CONTRIB</span>** | C |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |  |
| 6970 | [pgstattuple](/stat/pgstattuple) | 1.5 | [pgstattuple](/stat/pgstattuple) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcblue">CONTRIB</span>** | **<span class="tcblue">CONTRIB</span>** | C |  |  |  |  | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |  |
| 6980 | [auto_explain](/stat/auto_explain) | - | [auto_explain](/stat/auto_explain) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcblue">CONTRIB</span>** | **<span class="tcblue">CONTRIB</span>** | C |  |  |  | <span class="tcred">❗</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> | <span class="tcwarn">✘</span> |  |
| 6990 | [pg_stat_statements](/stat/pg_stat_statements) | 1.10 | [pg_stat_statements](/stat/pg_stat_statements) | **<span class="tcblue">PostgreSQL</span>** | **<span class="tcblue">CONTRIB</span>** | **<span class="tcblue">CONTRIB</span>** | C |  |  |  | <span class="tcred">❗</span> | <span class="tcblue">✔</span> | <span class="tcblue">✔</span> | <span class="tcwarn">✘</span> |  |


