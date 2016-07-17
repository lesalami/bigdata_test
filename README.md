# bigdata_test
Transfrom Data using PySpark

Simple Transformation

date;type;value

2016-07-01;impressions;1000

2016-07-01;impressions;100

2016-07-01;clicks;20

2016-07-01;conversions;1

2016-07-02;impressions;20

2016-07-02;clicks;2

2016-07-04;impressions;10

Data transformed to:

date;impressions;clicks;conversions

2016-07-01;1100;20;1

2016-07-02;20;2;null

2016-07-03;null;null;null

2016-07-04;10;null;null

#Approach
Decided to use Spark to show my Big Data skillset. Load the file from HDFS into context(sc) and then convert to a dataframe. Manipulate the data using Sparks sqlContext.
Write the aggregated transformed data to file.(Could can be run on Databricks here https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1124054440194824/3765384094733164/3328767132102979/latest.html
