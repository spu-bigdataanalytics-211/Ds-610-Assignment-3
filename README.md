# assignment-3
Apache Spark Practices

## Description

Use Apache Spark to find the answer for the following questions.

1. Find the # of flights each airline made so far  from 1987 until recent.
2. Find the mean departure delay per origination airport.
3. What is the average departure delay from each airport?
4. What day the delays are the worst?
5. Which day of the week is the most of the flights cancelled?
6. Which day of the month is the most of the flights cancelled?
7. Find the on-time (ArrTime - CRSArrTime <= 0) performance for each unique carrier.

## Hints

If using Google Colab, attach Google drive to Google Colab.

``` py
from google.colab import drive
drive.mount('/content/drive')
```

Read all files in single code.

``` py
sc = spark.sparkContext
rdd = sc.textFile('/content/drive/path/to/files/*.csv.bz2')
```

Use `.take()` or `.first()` instead of `.collect()`.

``` py
rdd.take(2)
```

## Dataset

Dataset is same as assignment 2, use if from the Google Drive folder. Use [spu-bigdataanalytics-211/assignment-2](https://github.com/spu-bigdataanalytics-211/assignment-2) to see more on data dictionary.

You can find more information about this dataset in the website of [Statistical Computing](http://stat-computing.org/dataexpo/2009/). Find out more information on [Airline On-Time Performance Data](https://www.transtats.bts.gov/DatabaseInfo.asp?QO_VQ=EFD&QO_anzr=Nv4yv0r%20b0-gvzr%20cr4s14zn0pr%20Qn6n) from [Bureau of Transportation Statistics (BTS)](https://www.transtats.bts.gov/).

## How to work on this Assignment?

1. Download this repository with `git clone https://github.com/spu-bigdataanalytics-211/assignment-3.git`.
2. [Create a virtual environment](#how-to-create-a-new-virtual-environment) and activate this environment everytime you need to use it.
3. Install [requirements.txt](requirements.txt) file using `pip install -r requirements.txt`.
4. Create a notebook.

## Questions

The repository should be self descriptive and it should guide you through assignment. Let me know if you have any questions.
