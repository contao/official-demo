# How to update the COD

## Contao
- use last version of COD and import fresh SQL template
- update Contao to new version und update database (use release alias of COD for version to avoid errors)
- export database (see configuration `SQL Export.png`: only export data, remove `tl_log`, `tl_search`, `tl_search_index`)

## SQL
- archive old SQL file (move to folder `sql-archive`)
- create new SQL file in folder `src\templates\` with format `codvX.X.X_contao_Y.Y.Y.sql` (X.X.X is the new COD version, Y.Y.Y the min Contao version)
- insert SQL content from export

## `composer.json`
- define min version für `core-bundle`
- update referenced SQL file name

## Theme Import
- use export function in backend and replace file `src\files\contaodemo\contao_official_demo.cto`