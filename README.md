# sample
テストで使用したサンプルプログラムです。
ほとんどの物は、利用価値のないものですが、自分の健忘録や事象の説明などのために作成しました。

# oon.java 
Java HotSpot コンパイラが、 "COMPILE SKIPPED: out of nodes during split" でスキップする様子を確認する目的のサンプルです。
短いコードで確認できる良い方法が思いつかず、延々と意味の無い長いコードになってしまいました。

$ javac oon.java
$ java -XX:+PrintCompilation oon で起動すると COMPILE SKIPPED の状況が確認できました。
...
   7302   19             oon::challenge (7992 bytes)   COMPILE SKIPPED: out of nodes during split (not retryable)
...
※ RHEL 7.4 + java 1.7.0_141 の環境にて
