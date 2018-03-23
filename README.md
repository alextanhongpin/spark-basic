# spark-basic
Basic Apache Spark tutorials

## Installation

```bash
$ brew install apache-spark
```

## Version

```bash
$ pyspark --version

Welcome to
      ____              __
     / __/__  ___ _____/ /__
    _\ \/ _ \/ _ `/ __/  '_/
   /___/ .__/\_,_/_/ /_/\_\   version 2.3.0
      /_/

Using Scala version 2.11.8, Java HotSpot(TM) 64-Bit Server VM, 1.8.0_131
Branch master
Compiled by user sameera on 2018-02-22T19:24:29Z
Revision a0d7949896e70f427e7f3942ff340c9484ff0aab
Url git@github.com:sameeragarwal/spark.git
Type --help for more information.
```

## Configure PySpark to use Jupyter Notebook

In your `.bashrc` or `.zshrc` file:

```
export PYSPARK_DRIVER_PYTHON=jupyter
export PYSPARK_DRIVER_PYTHON_OPTS='notebook'
export PYSPARK_PYTHON=/usr/local/Cellar/python/3.6.4/bin/python3
```

Restart your terminal, and running `pyspark` will now open the Jupyter Notebook.

```bash
# To get the path to the python version
$ brew info python
```
