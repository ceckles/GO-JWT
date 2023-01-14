GO API Server with JWT Authentication
====================================
This is a simple example of how to use JWT Authentication in a Go API Server.

The server is built using the [Gin](github.com/gin-gonic/gin) framework.
and a mongodb database. provided by [MongoDb](https://www.mongodb.com/)

I have encluded a same postman collection to test the API.

##.env file
```
PORT=9000
MONGODB_URL=BDURLGOESHERE
CLUSTER=CLUSTERNAMEGOESHERE(eg:cluster0)
SECRET_KEY=SECRETKEYGOHERE
```

##Installation
```bash
go get github.com/gin-gonic/gin
go get go.mongodb.org/mongo-driver/mongo
go get github.com/dgrijalva/jwt-go
go get github.com/joho/godotenv
go get github.com/go-playground/validator/v10
go get golang.org/x/crypto/bcrypt"

# not tried but should work
go get ./...

```

##Run
```bash
go run main.go
```