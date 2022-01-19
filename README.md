# truetool
A easy tool for frequently used TrueNAS SCALE CLI utilities.
Previously known as "trueupdate"

## How to install

run `pip install truetool`

Please be aware you will need to reinstall after every SCALE update

## How to Update

run `pip install --upgrade truetool`

## How to use

running `truetool` should be a good start.

Additional options are available:

##### Help

- `truetool -h` for the CLI help page


##### Update

- `truetool -u` or ` truetool --update` update TrueNAS SCALE Apps


- `truetool --catalog CATALOGNAME` where CATALOGNAME is the name of the catalog you want to process in caps
- `truetool --versioning SCHEME` where SCHEME is the highest semver version you want to process. options: `patch`, `minor` and `major`
- `truetool -a` or ` truetool --all` updates both active (running) and non-active (stuck or stopped) Apps


#### Backup
- `truetool -b` or ` truetool --backup` backup the complete Apps system prior to updates
- `truetool -r` or ` truetool --restore` restores a specific backup by name

#### Other

- `truetool -s` or ` truetool --sync` to sync the catalogs before running updates
- `truetool -p` or ` truetool --prune` to prune (remove) old docker images after running auto-update