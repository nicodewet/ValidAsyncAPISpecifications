# ValidAsyncAPISpecifications

A collection of AsyncAPI Specifications that are guaranteed to be valid.

Why? Because starting with an invalid specification can waste precious time.

Validation was performed using:

```
% docker run --rm -it --user=root asyncapi/cli --version                                 

@asyncapi/cli/1.1.3 linux-arm64 node-v16.20.2
```

Validation example:

```
% docker run --rm -it \
-v ./hoboken-district-station-capacity-asyncapi-2.4.0.yml:/app/asyncapi.yml \
asyncapi/cli validate
```