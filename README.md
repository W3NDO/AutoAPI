# AutoAPI

This is a basic project that takes in a JOSN file and generates a REST API with the specifications in the project. 

## JSON format
Run the script in a folder with a file named `endpoints.json`
```
{
    "GET": {
        "endpoint_name": {
            "query_params": [],
            "header": {"Content-Type": "application/json"},
            "response": {
                "content": {"message": "Hello AutoAPI"},
                "file": false
            }
        },
    },
    "POST": {
        "endpoint_name": { 
            "header": {},
            "body": {},
            "query_params": {}
        }
    },
    "PUT": {
        "endpoint_name": { 
            "header": {},
            "body": {},
            "query_params": {}
        }
    },
    "DELETE": {
        "endpoint_name": { 
            "header": {},
            "body": {},
            "query_params": {}
        }
    }
}
```

## Running the script

Define your `endpoints.json` file. For now we only support `GET` requests.

Make the file executable. On linux it would be `chmod +x autoapi`

Then run it. `./autoapi`
