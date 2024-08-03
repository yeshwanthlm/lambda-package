# Required Commands to Deploy Python Code along with Dependent Packages to AWS Lambda

```bash
mkdir lambda_deployment

cd lambda_deployment/

vi lambda_function.py

pip install requests -t .

zip -r ../lambda_package.zip .

aws s3 cp lambda_package.zip s3://{bucket_name}
```
