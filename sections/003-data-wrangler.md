### Where does Data Wrangler fit within SageMaker?

Data Wrangler makes it easy for you to collect and prepare the data you need to build ML models. Without writing a single line of code, Amazon SageMaker Data Wrangler can automatically transform your data into new features.

Data Wrangler’s data selection tool easily integrates with multiple data sources like Amazon Athena, Amazon Redshift, AWS Lake Formation, Amazon S3, and Amazon SageMaker Feature Store. You can write queries for data sources and import data directly into SageMaker from various file formats, such as CSV files, parquet files, and database tables. This data is imported into a secure central data preparation environment where users will have access to a variety of pre-built tools to prepare their data.

To transform your data, SageMaker Data Wrangler offers a rich selection of pre-configured data transforms, such as convert column type, rename column, and delete column. For example, you can convert a text field column into a numerical column with a single click, or author custom transforms in PySpark, SQL, and Pandas to provide flexibility across your organization. This streamlines the process of cleaning, verifying, and visualizing data without writing a single line of code.

Once the data is transformed, SageMaker Data Wrangler makes it easy to clean and explore the data with data visualizations in SageMaker Studio. These visualizations allow you to quickly identify inconsistencies in data preparation workflow and diagnose issues before models are deployed into production. 

Finally, Data Wrangler makes it easy to create a pipeline for data preparation. Export your data preparation workflow to a notebook or code script with a single click to efficiently bring your data preparation workflows into production without manually sifting through and translating hundreds of lines of data preparation code. 


### Getting Started with Data Wrangler

Let’s get started with Data Wrangler. In the AWS Management Console, head over to the SageMaker page. On the dashboard page, select **Open SageMaker Domain.**
[Image: 1-open-sm-domain.PNG]You should see a user associated with a domain. Select **Launch app**, and then **Studio** from the user profile.

[Image: 2-launch-sm-studio.PNG]You will be redirected to SageMaker Studio. You can see all the SageMaker Studio has to offer. For now, select the triangle icon on the left-hand side for **SageMaker resources**. Then, select **Data Wranger** from the drop-down menu as a new SageMaker resource. Select **new flow** to initialized Data Wrangler. This can take a few minutes to complete. Refer to the screenshot if you need help. 
[Image: image.png]Once initialized, you will have the option to select your data source. Because our data is in Amazon S3, select **Amazon S3** to import data. Navigate to the S3 bucket and then the hotel books CSV file path. Data Wrangler will show you a preview of the data. You can specify the file type as CSV on the right side of the IDE. Select **Advanced configurations** then de-select **enable sampling**. Our data set is small enough to run Data Wrangler transformations on the full data set. If you have a large data set, consider using sampling. Finally select **Import** to finishing importing the data.

[Image: image.png]You’re now set up to start using Data Wrangler!