﻿# How to update the COD

## Contao
- use last version of COD and import fresh SQL template
- update Contao to new version und update database (use newly created branch alias, e.g. `dev-release/x.x.x` of COD for version to avoid errors)
- export database (see configuration `SQL Export.png`: only export data, remove `tl_crawl_queue`, `tl_cron_job`, `tl_log`, `tl_search`, `tl_search_index`, `tl_search_term`, `tl_undo`, `tl_version`)

## SQL
- archive old SQL file (move to folder `sql-archive`)
- create new SQL file in folder `src\templates\` with format `official-demo-for-contao-X.X.X` (X.X.X the min Contao version the demo is tested for)
- insert SQL content from export

## `composer.json`
- define min version für `core-bundle`
- update referenced SQL file name

## Theme Import
- use export function in backend and replace file `src\files\contaodemo\contao_official_demo.cto`