# Remove Example

## I Install NWA

```shell
go install github.com/B1NARY-GR0UP/nwa@latest
```

Verify the installation by type in following command and the version is display correctly.

```shell
nwa --version
```

## II Remove License Header

Remove license header for the go files under the `nwa-examples/remove` folder with following command.

```shell
cd remove
nwa remove -t tmpl.txt dirA dirB main.go
```

OR

```shell
cd add
nwa remove -t tmpl.txt README.md .
```

## III Check

Now all the go files under `nwa-examples/add` do not have a license header, NWA runs correctly.
