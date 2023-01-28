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
