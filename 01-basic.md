# Basic


```bash
$ pyspark

# Read text file
>>> textfile = spark.read.text('./README.md')
2018-03-23 16:46:15 WARN  ObjectStore:6666 - Version information not found in metastore. hive.metastore.schema.verification is not enabled so recording the schema version 1.2.0
2018-03-23 16:46:15 WARN  ObjectStore:568 - Failed to get database default, returning NoSuchObjectException
2018-03-23 16:46:16 WARN  ObjectStore:568 - Failed to get database global_temp, returning NoSuchObjectException

# Number of rows in this DataFrame
>>> textfile.count()
28

# First row in this DataFrame
>>> textfile.first()
Row(value=u'# spark-basic')

# Create a new DataFrame that contains the text spark
>>> linesWithSpark = textfile.filter(textfile.value.contains('spark'))
.
>>> linesWithSpark.count()
4
```

