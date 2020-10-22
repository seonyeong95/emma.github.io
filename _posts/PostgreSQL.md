---
title: "PostgreSQL"
date: 2020-10-22 13:00:00 -0400
categories: R
---


​```python
# db불러오기
library(DBI)
library(RPostgreSQL)

con<-dbConnect(dbDriver("PostgreSQL"),dbname = "",host = "",
               user = "", password = "")
recordSet<-dbSendQuery(con, "select * from bbp_prd_tabown.tbbp10_cc_01_201902")
data<-dbFetch(recordSet)
​```

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
