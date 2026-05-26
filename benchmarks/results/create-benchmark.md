```

BenchmarkDotNet v0.15.8, Linux Ubuntu 24.04.4 LTS (Noble Numbat)
AMD EPYC 9V74 2.60GHz, 1 CPU, 4 logical and 2 physical cores
.NET SDK 10.0.300
  [Host]   : .NET 10.0.8 (10.0.8, 10.0.826.23019), X64 RyuJIT x86-64-v3
  ShortRun : .NET 10.0.8 (10.0.8, 10.0.826.23019), X64 RyuJIT x86-64-v3


```
| Method                                      | Mean       | StdDev   | Error     | Gen0       | Gen1       | Gen2      | Allocated  |
|-------------------------------------------- |-----------:|---------:|----------:|-----------:|-----------:|----------:|-----------:|
| &#39;MiniExcel Create Xlsx with Simple Mapping&#39; |   688.7 ms |  6.63 ms | 120.95 ms | 23666.6667 |  1333.3333 | 1333.3333 |  372.15 MB |
| &#39;MiniExcel Create Xlsx&#39;                     |   733.2 ms |  3.92 ms |  71.58 ms | 27500.0000 |  1666.6667 | 1500.0000 |   432.7 MB |
| &#39;ClosedXml Create Xlsx&#39;                     | 1,600.1 ms | 14.64 ms | 267.12 ms | 21833.3333 |  8000.0000 | 2833.3333 |  401.23 MB |
| &#39;OpenXmlSdk Create Xlsx by DOM mode&#39;        | 2,069.2 ms | 13.45 ms | 245.41 ms | 45166.6667 | 45000.0000 | 3333.3333 |   762.9 MB |
| &#39;Epplus Create Xlsx&#39;                        | 2,295.8 ms |  7.09 ms | 129.34 ms | 12166.6667 |  6333.3333 | 4166.6667 |  288.25 MB |
| &#39;NPOI Create Xlsx&#39;                          | 3,707.9 ms | 22.62 ms | 412.60 ms | 98833.3333 | 48333.3333 | 3000.0000 | 1748.04 MB |
