# マルチスレッドとマルチプロセス

## 【事前理解】並行(Concurrent)と並列(Parallel)について

> https://twitter.com/tnmt/status/318211278810275840
> 
> 分かりやすい RT @hiboma: 羽生さんが将棋の多面指しで小学生100人を一気に相手しているのが concurrent 将棋,  羽生さんが増えて N人 (N≧2) になると parallel 将棋

Concurrent ⊃ Parallel (※⊇かもしれない)

Concurrentは実行状態の複数保持を意味しており、Parallelは実行状態の複数保持、かつ同時実行の可能を意味している。

### 並行的とは

```text
+-----+
| CPU | [  job1  ] [  job2  ]
+-----+
        --------------------------------------->
        time
```

### 並列的とは

```text
+------+
| CPU1 | [  job1  ]
+------+
+------+
| CPU2 | [  job2  ]
+------+
         --------------------------------------->
         time
```