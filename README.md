# xgb_python_vs_r

the xgb.cv in python and r is different<br>

for example:<br>
# we train iris dataset by xgb.cv in R <br> 
```sh
[2]     train-merror:0.056667+0.028674  test-merror:0.040000+0.028284 
[3]     train-merror:0.040000+0.016330  test-merror:0.046667+0.024944 
Stopping. Best iteration:
[2]     train-merror:0.056667+0.028674  test-merror:0.040000+0.028284
```
# train iris by xgb.cv in Python <br>
```sh
   train-merror-mean  test-merror-mean
           0.046667          0.046667
```

the params of r and python are same <br>

```sh
xgb_params=list( 	
  objective="multi:softmax",
  eta= 0.01, 
  max_depth= 1, 
  colsample_bytree= 0.7,
  subsample = 0.7
  num_class = 3)
```
<br><br>
results are different, if we use other data, that will more different, but we don't know why
<br><br><br>


================================================<br>
PS:<br>
# R version 3.3.3 (2017-03-06)   <br>
Platform: x86_64-pc-linux-gnu (64-bit)<br>
Running under: Ubuntu 16.04.2 LTS<br>
<br>
locale:<br>
 [1] LC_CTYPE=zh_TW.UTF-8       LC_NUMERIC=C               LC_TIME=zh_TW.UTF-8       <br>
 [4] LC_COLLATE=zh_TW.UTF-8     LC_MONETARY=zh_TW.UTF-8    LC_MESSAGES=zh_TW.UTF-8   <br>
 [7] LC_PAPER=zh_TW.UTF-8       LC_NAME=C                  LC_ADDRESS=C              <br>
[10] LC_TELEPHONE=C             LC_MEASUREMENT=zh_TW.UTF-8 LC_IDENTIFICATION=C       <br>
<br>
attached base packages:<br>
[1] stats     graphics  grDevices utils     datasets  methods   base     <br>
<br>
other attached packages:<br>
[1] Matrix_1.2-8      mice_2.30         timeDate_3012.100 xgboost_0.6-4     dplyr_0.5.0      <br>
[6] data.table_1.10.4<br>
<br>
loaded via a namespace (and not attached):<br>
 [1] Rcpp_0.12.10    lattice_0.20-35 assertthat_0.1  MASS_7.3-45     grid_3.3.3     <br>
 [6] R6_2.2.0        DBI_0.6-1       magrittr_1.5    stringi_1.1.5   rpart_4.1-10   <br>
[11] splines_3.3.3   tools_3.3.3     survival_2.41-3 nnet_7.3-12     tibble_1.3.0  <br>

<br>
# python<br>
xgb.__version__<br>
Out[107]: '0.6'







