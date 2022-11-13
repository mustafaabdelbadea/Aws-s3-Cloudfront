
- Origin Domain:
	my-static-website-bucket01.s3-website-us-east-1.amazonaws.com


- Index document Entry point
	index.html

- Bucket policy permission
	{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "AddPerm",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::my-static-website-bucket01/*"
        }
    ]
}

- aws Cloudfront url
https://d7e7mw3d2fak5.cloudfront.net/

**Note That url may not working if bucket deleted