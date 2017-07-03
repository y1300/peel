# peel
front-end for juicer

## install elasticbeanstalk
```
(venv)~$ pip install --upgrade awsebcli
```
Verify that the EB CLI is installed correctly.
```
$ eb --version

```
## [How to change the AWS account using the Elastic Beanstalk CLI](https://stackoverflow.com/questions/29190202/how-to-change-the-aws-account-using-the-elastic-beanstalk-cli)

The awsebcli tool automatically creates a file named ~/.aws/config and you can see your keys in there under the [profile eb-cli] category. Just change them there.

```
[profile eb-cli]
aws_access_key_id = ...
aws_secret_access_key = ...
```

## To initialize an EB CLI project (interactively)
```
$ eb init -i
```

## To create new invironment
```
eb create
```
check
```
eb status
```



## deploy changes to awseb without committing

Add new and changed files to the staging area:
```
~/peel$ git add .
```
Deploy the staged changes with eb deploy:
```
~/peel$ eb deploy --staged
```
