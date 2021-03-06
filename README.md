# Python boto3 script for creating buckets on aws s3
![python_boto3](https://user-images.githubusercontent.com/52320907/127744201-51dd1b60-6a89-4c9d-9f3c-b475a3576d18.png)
## instructions - how to run this python script
1) First install boto3

```
pip install boto3
```
2) Create a new user on aws console <a href="https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html">Creating an IAM user in your aws account</a>

3) Make sure during the proccess of creating a new user, enable "programmatic access" and add the following permission "AmazonS3FullAccess"

4) Add the following permission "AmazonS3FullAccess"

5) After the creation of the user, you will need to configure his credentials in your locall machine as follow:
```
touch ~/.aws/credentials
```
6) Open the file you created in the previous step and paste the following configuration:
```
[default]
aws_access_key_id = YOUR_ACCESS_KEY_ID
aws_secret_access_key = YOUR_SECRET_ACCESS_KEY
```
7) Make sure to add your ACCESS_KEY_ID and SECRET_ACCESS_KEY of the new user

8) Create another config file for configuring your region
```
touch ~/.aws/config
```
9) Download the script from the current repo to your machine and run it
```
python boto3_s3_connect.py
```
