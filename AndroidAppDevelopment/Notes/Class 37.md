## Reading

[Introduction to Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/dev/Introduction.html)

1. What is Amazon S3?
	1.  Amazon S3 (Simple Storage Service) is a scalable cloud storage service provided by Amazon Web Services (AWS). It allows individuals and businesses to store and retrieve large amounts of data in a secure and highly available manner.
2. List at least 3 features that it offers to its users.
	 Amazon S3 offers the following features to its users:

	1. Scalability and Durability: Amazon S3 can store virtually unlimited amounts of data and automatically scales to accommodate growing storage needs. It is designed to provide high durability, ensuring that data is protected against failures and can be accessed reliably.

	2. Data Security and Access Control: S3 provides robust security features to protect stored data. It supports encryption of data at rest and in transit, access control policies, and integrates with AWS Identity and Access Management (IAM) for fine-grained access control.

	3. Data Management and Lifecycle Policies: S3 offers features for managing data lifecycle, including lifecycle policies that allow you to automate the transition of objects to different storage classes based on defined rules. It also provides versioning capabilities
3. What is an object key?
	1. An object key in Amazon S3 is a unique identifier assigned to each object (file) stored in an S3 bucket. It acts as the unique address or name of the object and is used to retrieve and manage the object within the bucket. The object key consists of the full path and filename of the object, which allows for easy organization and retrieval of objects stored in S3.

[S3 with Amplify](https://docs.amplify.aws/lib/storage/getting-started/q/platform/android/)

1. Which dependencies are needed to install Amplify AWS S3 to your android application?
	1. implementation 'com.amplifyframework:aws-storage-s3:1.17.4' 
	2. implementation 'com.amplifyframework:aws-auth-cognito:1.17.4'
2. What is needed in order to upload data to your bucket?
	 In order to upload data to your Amazon S3 bucket using Amplify, you need the following:
    
    2. AWS Configuration: Set up the required AWS credentials and configuration, such as AWS access key, secret key, and the desired AWS region. These configurations should be properly configured in your Android application.
    
    2. Amplify Initialization: Initialize the Amplify framework in your application by calling `Amplify.addPlugin()` and `Amplify.configure()`. This ensures that Amplify is properly set up to work with AWS services.
    
    3. File Upload Process: Use Amplify's Storage category to upload data to your bucket. This involves specifying the file path, destination key, and optional metadata or access control settings for the uploaded file.
3. what method(s) initialize(s) the Amplify Auth and Storage categories?
		The Amplify Auth and Storage categories can be initialized using the following methods:
    
    1. Amplify Auth: To initialize the Amplify Auth category, you need to call `Amplify.addPlugin(new AWSCognitoAuthPlugin())` to add the AWS Cognito Auth plugin, and then call `Amplify.configure(context)` to configure Amplify with the appropriate context.
    
    2. Amplify Storage: To initialize the Amplify Storage category, you need to call `Amplify.addPlugin(new AWSS3StoragePlugin())` to add the AWS S3 Storage plugin, and then call `Amplify.configure(context)` to configure Amplify with the appropriate context.
    
    These initialization methods ensure that the Amplify Auth and Storage categories are properly set up and ready to be used in your Android application.