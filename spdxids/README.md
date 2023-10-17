# SPDX IDs Example

## I Install NWA

```shell
go install github.com/B1NARY-GR0UP/nwa@latest
```

Verify the installation by type in following command and the version is display correctly.

```shell
nwa --version
```

## II Add SPDX IDs

Add SPDX IDs header for the go files under the `nwa-examples/spdxids` folder with following command.

```shell
cd spdxids
nwa add -i "Apache and MIT" main.go
```

## III Check

Now all the go files under `nwa-examples/spdxids` have a SPDX IDs header, NWA runs correctly.
