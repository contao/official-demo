# How to update the COD

## Contao
- use last version of COD and import fresh SQL template
- update Contao to new version und update database
- export database (see configuration, remove `tl_log` entry)
![configure export for phpMyAdmin][SQL Export.png]

## SQL
- archive old SQL file (move to folder `sql-archive`)
- create new SQL file in folder `src\templates\` with format `codvX.X.X_contao_Y.Y.Y.sql` (X.X.X is the new COD version, Y.Y.Y the min Contao version)
- insert SQL content from export

## `composer.json`
- define min version für `core-bundle`
- update referenced SQL file name

## Theme Import
- use export function in backend and replace file `src\files\contaodemo\contao_official_demo.cto`