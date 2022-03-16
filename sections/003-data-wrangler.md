### Where does Data Wrangler fit within SageMaker?

Data Wrangler makes it easy for you to collect and prepare the data you need to build ML models. Without writing a single line of code, Amazon SageMaker Data Wrangler can automatically transform your data into new features.

Data Wrangler’s data selection tool easily integrates with multiple data sources like Amazon Athena, Amazon Redshift, AWS Lake Formation, Amazon S3, and Amazon SageMaker Feature Store. You can write queries for data sources and import data directly into SageMaker from various file formats, such as CSV files, parquet files, and database tables. This data is imported into a secure central data preparation environment where users will have access to a variety of pre-built tools to prepare their data.

To transform your data, SageMaker Data Wrangler offers a rich selection of pre-configured data transforms, such as convert column type, rename column, and delete column. For example, you can convert a text field column into a numerical column with a single click, or author custom transforms in PySpark, SQL, and Pandas to provide flexibility across your organization. This streamlines the process of cleaning, verifying, and visualizing data without writing a single line of code.

Once the data is transformed, SageMaker Data Wrangler makes it easy to clean and explore the data with data visualizations in SageMaker Studio. These visualizations allow you to quickly identify inconsistencies in data preparation workflow and diagnose issues before models are deployed into production. 

Finally, Data Wrangler makes it easy to create a pipeline for data preparation. Export your data preparation workflow to a notebook or code script with a single click to efficiently bring your data preparation workflows into production without manually sifting through and translating hundreds of lines of data preparation code. 