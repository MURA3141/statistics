# statistics

# バイオリンプロットを書くためのRコード＜br＞
データの入力 <br>

data <- data.frame(
+     category = c("Healthy", "Healthy","Healthy","Healthy","Healthy","Healthy", "Exercise", "Exercise","Exercise","Exercise","Exercise","Exercise"),
+   value = c(10, 13, 11, 18, 8, 20,27,26,25,31,35,32)
+ )<br>
<br>
このデータは"Healthy", "Exercise",が6サンプルずつ、Valueの数値を得たというコード<br>
まずは、バイオリンプロットを書いてみる<br>

> 
> p <- ggplot(data, aes(x=category, y=value)) + 
+     geom_violin(trim=FALSE, fill="lightblue") +
+     labs(x="Category", y="Value") +
+     theme_minimal()
> 
> p + geom_jitter(position=position_jitter(width=0.2), shape=16) <br>
>
><img width="534" alt="スクリーンショット 2023-10-10 20 15 15" src="https://github.com/MURA3141/statistics/assets/131435195/0657c4bc-25fa-4db9-b996-949a2915ea33">


> 


