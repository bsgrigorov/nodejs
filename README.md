# Run of the mill NodeJS app

## Docker
```
docker build -t nodeapp .
docker run -p 3000:3000 -d nodeapp
```

## Run with Node
Get dependencies
```
npm ci
```

Run
```
npm run start
```

## Cloudformation
Create OIDC stack
```
aws cloudformation create-stack --stack-name github-oidc --template-body file:///${PWD}/cf.template --parameters ParameterKey=GitHubOrg,ParameterValue=bsgrigorov ParameterKey=RepositoryName,ParameterValue=nodejs --capabilities CAPABILITY_IAM
```
