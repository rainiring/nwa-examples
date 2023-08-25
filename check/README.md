# Check Example

## I Install NWA

```shell
go install github.com/B1NARY-GR0UP/nwa@latest
```

Verify the installation by type in following command and the version is display correctly.

```shell
nwa --version
```

## II Add License Header

Check the go file under the `nwa-examples/check` folder if they have a expected license header as following.

```text

```

```shell
cd add
nwa add -l apache -c "RHINE LAB.LLC." -y 2077 dirA dirB main.go
```

OR

```shell
cd add
nwa add -l apache -c "RHINE LAB.LLC." -y 2077 -s README.md .
```

## III Check

Now all the go files under `nwa-examples/add` have a license header, NWA runs correctly.
