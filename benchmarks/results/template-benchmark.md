```

BenchmarkDotNet v0.15.8, Linux Ubuntu 24.04.4 LTS (Noble Numbat)
AMD EPYC 9V74 2.87GHz, 1 CPU, 4 logical and 2 physical cores
.NET SDK 10.0.300
  [Host]   : .NET 10.0.8 (10.0.8, 10.0.826.23019), X64 RyuJIT x86-64-v3
  ShortRun : .NET 10.0.8 (10.0.8, 10.0.826.23019), X64 RyuJIT x86-64-v3


```
| Method                               | Mean         | StdDev     | Error        | Gen0        | Gen1       | Gen2      | Allocated  |
|------------------------------------- |-------------:|-----------:|-------------:|------------:|-----------:|----------:|-----------:|
| &#39;MiniExcel Mapping Fill Template&#39;    |     3.326 ms |  0.0849 ms |     1.548 ms |   2770.8333 |  2744.7917 | 2744.7917 |    15.4 MB |
| &#39;MiniExcel Fill Template&#39;            |   471.199 ms |  4.1946 ms |    76.526 ms |  37333.3333 |   333.3333 |         - |  596.88 MB |
| &#39;ClosedXml.Report Generate Template&#39; | 5,215.959 ms | 61.5407 ms | 1,122.732 ms | 169333.3333 | 56333.3333 | 6500.0000 | 2799.89 MB |
