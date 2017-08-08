# AWS CLI on Docker

Execute aws command on Docker.

## Usage

Example of `aws s3 ls` command.

```bash
export AWS_ACCESS_KEY_ID="XXXXXXXX"
export AWS_SECRET_ACCESS_KEY="YYYYYYYY"
export AWS_DEFAULT_REGION="ZZZZZZZZ"

docker run --rm \
	-e "AWS_ACCESS_KEY_ID=$AWS_ACCESS_KEY_ID" \
	-e "AWS_SECRET_ACCESS_KEY=$AWS_SECRET_ACCESS_KEY" \
	-e "AWS_DEFAULT_REGION=$AWS_DEFAULT_REGION" \
	lorentzca/aws s3 ls
```
