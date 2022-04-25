---
title: "Amazon S3"
weight: 312
---

# Import data from Amazon S3


Data Wrangler uses S3 Select to allow you to preview your Amazon S3 files in Data Wrangler. 

You can import single files in the following formats:

    Comma Separated Values (CSV)

    Parquet

    Javascript Object Notation (JSON)

    Optimized Row Columnar (ORC)



When you choose a dataset, you can rename it, specify the file type, and identify the first row as a header.

You can import either a single file or multiple files as a dataset. You can use the multifile import operation when you have a dataset that is partitioned into separate files. It takes all of the files from an Amazon S3 directory and imports them as a single dataset. 

# Steps

We will be uploading sample data file into S3. We will then import the data into Datawrangler

### Download the sample data file: 
![Sample data](https://github.com/neelamkoshiya/DataWrangler/blob/main/hotel_bookings.csv)

### Create S3 bucket 
* Sign in to the AWS Management Console and open the Amazon S3 console at https://console.aws.amazon.com/s3/

* Choose Create bucket.

* The Create bucket wizard opens.

In Bucket name, enter a DNS-compliant name for your bucket.

The bucket name must:

    Be unique across all of Amazon S3.

    Be between 3 and 63 characters long.

    Not contain uppercase characters.

    Start with a lowercase letter or number.

* Keep everything default and Choose Create bucket.

### Upload the sample


* In the Buckets list, choose the name of the bucket that you created in previous step.

* On the Objects tab for your bucket, choose Upload.

* Under Files and folders, choose Add files.

* Choose hotel_bookings.csv which you downloaded in the previous step and then choose Open.

* Choose Upload.

### Import in Data Wrangler

Prequisite: To use Data Wrangler, you need an active Studio instance. To learn how to launch a new instance, see [Onboard to Amazon SageMaker Domain](https://docs.aws.amazon.com/sagemaker/latest/dg/onboard-quick-start.html). When your Studio instance is Ready, use the below instructions.

* To access Data Wrangler in Studio:

Next to the user you want to use to launch Studio, select Open Studio.

* When Studio opens, select the + sign on the New data flow card under ML tasks and components. This creates a new directory in Studio with a .flow file inside, which contains your data flow. The .flow file automatically opens in Studio.
![ds1](/static/ds1.png)

* When you create a new .flow file in Studio, you may see a message within the Data Wrangler interface that says:

"Data Wrangler is loading..." This may take a few minutes.
![ds2](/static/ds2.png)

* Click on Amazon S3

![ds3](/static/ds3.png)

* Select the bucket which you created in previous step

![ds4](/static/ds4.png)

* Select the CSV file and click Import

![ds5](/static/ds5.png)

![ds6](/static/ds6.png)


Congratulations, you have successfully imported the sample data file from S3 into Data Wrangler

