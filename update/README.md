# Update Example

## I Install NWA

```shell
go install github.com/B1NARY-GR0UP/nwa@latest
```

Verify the installation by type in following command and the version is display correctly.

```shell
nwa --version
```

## II Update License Header

Update copyright holder and copyright year of the source code under the `nwa-examples/update` folder with following command.

```shell
cd update
nwa update -l mit -c "BINARY-Members" -s README.md .
```

## III Check

Now all the source code files under `nwa-examples/update` have the updated license header, NWA runs correctly.
