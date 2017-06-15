# peer
front-end for juicer

## deploy changes to awseb without committing

Add new and changed files to the staging area:
```
~/peel$ git add .
```
Deploy the staged changes with eb deploy:
```
~/peel$ eb deploy --staged
```
