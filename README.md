# Avrogen namespace bug
The purpose of this project is to showcase a bug regarding namespace mapping in avrogen dotnet tool for Apache Avro.

For more information about the bug, see the bug report: [AVRO-2883](https://issues.apache.org/jira/browse/AVRO-2883)

## How to reproduce
1. Run `dotnet tool restore` in the root of the project dir, after cloning.
2. Run `dotnet build` which will run `dotnet avrogen -s $(ProjectDir)models.avsc $(ProjectDir) --namespace my.avro.ns:my.csharp.ns` before attempting to compile the project (the compilation will fail).