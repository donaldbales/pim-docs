# Akeneo PIM Documentation

The Akeneo PIM documentation

## Build the documentation

Install [Docker](https://docs.docker.com/engine/installation/).

Then `make build`.

The docs will be built into `./pim-docs-build`.

## Deploy the documentation

To deploy what you have built, use `HOSTNAME=foo.com PORT=1985 VERSION=bar make deploy`.

`HOSTNAME` is the server to deploy the documentation on.
`PORT` is the SSH port to connect to the server.
`VERSION` is the subdirectory of `/var/www/` where the documentation will be deployed on the the server. It should be something like `3.2`, `4.0` or `master`. 

To know the production and staging environments of pim-docs, please read the [inventory](https://github.com/akeneo/ansible/blob/master/inventories/core.inventory).

## Contribution

Don't hesitate to suggest cookbook ideas via https://github.com/akeneo/pim-docs/issues.

## Developer's notes

- The folder `/_themes/sphinx_rtd_theme` is a clone from https://github.com/snide/sphinx_rtd_theme, and was
updated on 2016-07. If you want to customize the Akeneo theme, please only update `/_theme/akeneo_rtd` theme.
