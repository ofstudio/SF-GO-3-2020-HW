# Модуль 12. Алгоритмы сортировки

```
% go test -bench=. -benchtime=10x ./...

goos: darwin
goarch: amd64
pkg: sf-golang-12/sort
cpu: Intel(R) Core(TM) i5-1030NG7 CPU @ 1.10GHz
...
```


## Массив со случайными значениями

| Алгоритм        | n=10 | n=1000 | n=100000 | RAM |
|-----------------|-----:|-------:|---------:|:---:|
| Bubble          |    3 |      7 |       11 | -   |
| Insertion       |    3 |      6 |       10 | -   |
| Merge           |    4 |      5 |        7 | +   |
| Quick           |    3 |      5 |        7 | -   |
| Selection       |    3 |      7 |       10 | -   |
| SelectionBidi   |    3 |      6 |       10 | -   |

## Предварительно отсортированный массив

| Алгоритм        | n=10 | n=1000 | n=100000 | RAM |
|-----------------|-----:|-------:|---------:|:---:|
| Bubble          |    3 |      4 |        6 | -   |
| Insertion       |    3 |      4 |        5 | -   |
| Merge           |    3 |      5 |        7 | +   |
| Quick           |    3 |      5 |        7 | -   |
| Selection       |    3 |      6 |       10 | -   |
| SelectionBidi   |    3 |      6 |       10 | -   |

## Предварительно отсортированный в обратном порядке массив

| Алгоритм        | n=10 | n=1000 | n=100000 | RAM |
|-----------------|-----:|-------:|---------:|:---:|
| Bubble          |    3 |      6 |       10 | -   |
| Insertion       |    3 |      6 |       10 | -   |
| Merge           |    3 |      5 |        7 | +   |
| Quick           |    3 |      6 |       10 | -   |
| Selection       |    3 |      6 |       10 | -   |
| SelectionBidi   |    3 |      6 |       10 | -   |

## Массив с предварительно отсортированными последовательностями

| Алгоритм        | n=10 | n=1000 | n=100000 | RAM |
|-----------------|-----:|-------:|---------:|:---:|
| Bubble          |    3 |      6 |       10 | -   |
| Insertion       |    3 |      6 |       10 | -   |
| Merge           |    4 |      5 |        7 | +   |
| Quick           |    3 |      5 |        7 | -   |
| Selection       |    4 |      6 |       10 | -   |
| SelectionBidi   |    3 |      6 |       10 | -   |
