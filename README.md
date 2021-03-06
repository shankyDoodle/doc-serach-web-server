# Doc Search Web Server
* This project creates a server which will serve all the HTTP requests from client.
* This is just a command line application so it can be tested using REST client or any other similar tool.

## Demo Link

This server is live on Amazon Web Services at 

[Web Server Live](http://3.16.149.228:1235/docs)

It's HTTP methods can be accessed via RESTclient.

## Run-Commands:
```bash
node ./index.js MONGO_DB_URL PORT NOISE_FILE [CONTENT_FILE...]
```

where
```bash
    MONGO_DB_URL
        Specifies the URL of the mongo database to be used for storing document information.

    PORT
        Specifies the port at which your program will listen for HTTP requests.

    NOISE_FILE
        Specifies a path to a file containing words which should be ignored within document content and searches.

    CONTENT_FILE...
        Specifies zero-or-more paths to files containing content which should be used for initializing the
        document collection.
```

## Pre-requisites:
MongoDb, Node.