# 名称：浏览日志
## 分支图显示

```code
$ git log --graph
$ git log --graph --oneline
```

## 显示最近几条记录

```code
$ git log -3 --pretty=oneline //显示3条日志
```

## 显示每次提交的具体改动

```code
// -p：可以在显示日志的同时显示改动
$ git log -p -l
```

## 显示每次更改的概要

```code
$ git log --stat --oneline
```

## 定制输出

```code
// --pretty=raw 显示commit的原始数据,可以
//显示提交对应的树ID
$ git log --pretty=raw -l
// --pretty=fuller 会同事显示作者和提交者
$ git log --pretty=fuller -l
// --pretty=oneline会提供最精剪的日志输出
$ git log --pretty=oneline -l
//如果只想查看和分析某一个提交，也可以使用git show
$ git show D --stat
//或者git cat-file,参数-p的含义是美观输出
$ git cat-file -p D^0

```
