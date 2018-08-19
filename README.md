Unorm Data Generator for unorm-dart
===

This is ported from [walling/unorm](https://github.com/walling/unorm) and modified to export unormdata for Dart language.

Development notes
-----------------

- [Unicode normalization forms report](http://www.unicode.org/reports/tr15/)
- Unicode data can be found from http://www.unicode.org/Public/UCD/latest/ucd

To generate new unicode data, run:
```sh
cd data/src
javac UnormNormalizerBuilder.java
java UnormNormalizerBuilder
```
produced `unormdata.data` contains needed table

Execute `node benchmark/benchmark.js` to run simple benchmarks, if you do any changes which may affect performance.
