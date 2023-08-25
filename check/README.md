# Check Example

## I Install NWA

```shell
go install github.com/B1NARY-GR0UP/nwa@latest
```

Verify the installation by type in following command and the version is display correctly.

```shell
nwa --version
```

## II Check License Header

Check the go file under the `nwa-examples/check` folder if they have an expected license header as following.

> fileA.go and fileB.go have the correct header;
> fileC.go's holder and year are incorrect;
> main.go does not have a license header;

```text
Copyright 2077 RHINE LAB.LLC.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

Execute following command which the flags match the expected license header.

```shell
cd check
nwa check -l apache -c "RHINE LAB.LLC." -y 2077 -s README.md .
```

## III Check

You will get the output log like following, we can know that `fileC.go` and `main.go` do not have a valid license header.

```text
time="2023-08-25T23:01:49+08:00" level=info msg="skip file" path=README.md
time="2023-08-25T23:01:49+08:00" level=info msg="file has a matched header" path="dirA\\fileA.go"                
time="2023-08-25T23:01:49+08:00" level=info msg="file does not have a matched header" path="dirB\\dirC\\fileC.go"
time="2023-08-25T23:01:49+08:00" level=info msg="file has a matched header" path="dirB\\fileB.go"                
time="2023-08-25T23:01:49+08:00" level=info msg="file does not have a matched header" path=main.go 
```
