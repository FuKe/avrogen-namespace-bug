# Avrogen namespace bug
This project is for showcasing a bug regarding namespace mapping in avrogen dotnet tool for Apache Avro.

## How to reproduce
1. Run `dotnet tool restore` in the root of the project dir, after cloning.
2. Run `dotnet build` which will run `dotnet avrogen -s $(ProjectDir)models.avsc $(ProjectDir)Models --namespace dk.aau.avrogen.test:AvroGenTest.Models` before attempting to compile the project (the compilation will fail).

TODO: Insert link to bug report.