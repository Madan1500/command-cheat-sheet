
# Serverless Framework Commands Quick Reference

## Installation

### Install the Serverless Framework
```bash
npm install -g serverless
```

### Install a specific version of the Serverless Framework
```bash
npm install -g serverless@<version>
```

---

## Project Setup

### Create a new service
```bash
sls create --template <templateName> --path <path>
```

### Create a new service with a specific runtime
```bash
sls create --template <templateName> --path <path> --runtime <runtime>
```

### Create a new service with a specific provider
```bash
sls create --template <templateName> --path <path> --provider <provider>
```

### Create a new service with a specific template and runtime
```bash
sls create --template <templateName> --path <path> --runtime <runtime>
```

### Create a new service with a specific template and provider
```bash
sls create --template <templateName> --path <path> --provider <provider>
```

### Create a new service with a specific runtime and provider
```bash
sls create --template <templateName> --path <path> --runtime <runtime> --provider <provider>
```

---

## Service Management

### Initialize a new service
```bash
sls init
```

### Initialize a new service with a specific template
```bash
sls init --template <templateName>
```

### Initialize a new service with a specific runtime
```bash
sls init --runtime <runtime>
```

### Initialize a new service with a specific provider
```bash
sls init --provider <provider>
```

### Initialize a new service with a specific template and runtime
```bash
sls init --template <templateName> --runtime <runtime>
```

### Initialize a new service with a specific template and provider
```bash
sls init --template <templateName> --provider <provider>
```

### Initialize a new service with a specific runtime and provider
```bash
sls init --runtime <runtime> --provider <provider>
```

### Initialize a new service with a specific template, runtime, and provider
```bash
sls init --template <templateName> --runtime <runtime> --provider <provider>
```

---

## Service Information

### Display information about the service
```bash
sls info
```

### Display information about the service with stage and region
```bash
sls info --stage <stage> --region <region>
```

---

## Function Management

### Create a new function
```bash
sls create function --name <functionName>
```

### Create a new function with a specific runtime
```bash
sls create function --name <functionName> --runtime <runtime>
```

### Create a new function with a specific handler
```bash
sls create function --name <functionName> --handler <handler>
```

### Create a new function with a specific runtime and handler
```bash
sls create function --name <functionName> --runtime <runtime> --handler <handler>
```

### Create a new function with a specific runtime, handler, and memory size
```bash
sls create function --name <functionName> --runtime <runtime> --handler <handler> --memorySize <memorySize>
```

### Create a new function with a specific runtime, handler, memory size, and timeout
```bash
sls create function --name <functionName> --runtime <runtime> --handler <handler> --memorySize <memorySize> --timeout <timeout>
```

---

## Function Information

### Display information about a function
```bash
sls info --function <functionName>
```

### Display information about a function with stage and region
```bash
sls info --function <functionName> --stage <stage> --region <region>
```

---

## Function Configuration

### Configure a function
```bash
sls config function --name <functionName>
```

### Configure a function with a specific runtime
```bash
sls config function --name <functionName> --runtime <runtime>
```

### Configure a function with a specific handler
```bash
sls config function --name <functionName> --handler <handler>
```

### Configure a function with a specific runtime and handler
```bash
sls config function --name <functionName> --runtime <runtime> --handler <handler>
```

### Configure a function with a specific runtime, handler, and memory size
```bash
sls config function --name <functionName> --runtime <runtime> --handler <handler> --memorySize <memorySize>
```

### Configure a function with a specific runtime, handler, memory size, and timeout
```bash
sls config function --name <functionName> --runtime <runtime> --handler <handler> --memorySize <memorySize> --timeout <timeout>
```

---

## Function Deployment

### Deploy a function
```bash
sls deploy function --function <functionName>
```

### Deploy a function with stage and region
```bash
sls deploy function --function <functionName> --stage <stage> --region <region>
```
---

## Deployment

### Deploy the entire service
```bash
sls deploy
```

### Deploy a single function
```bash
serverless deploy function --function functionName
```

### Deploy with stage and region
```bash
sls deploy --stage <stage> --region <region>
```

### Deploy the packaged service
```bash
sls deploy --package <path>
```



---

## Invocation

### Invoke a function locally
```bash
sls invoke local --function <functionName> --data '<JSON string>'
```

### Invoke a function remotely
#### First one is for when you have a JSON file with the event data and the second one is for when you have the event data as a JSON string.
```bash
serverless invoke --function functionName --path path/to/event.json
sls invoke --function <functionName> --data '<JSON string>'
```

### Invoke a function with a JSON file (locally)
```bash
sls invoke local --function <functionName> --path path/to/event.json
```

---

## Logs

### Fetch logs for a deployed function
```bash
sls logs --function <functionName>
```

### Tail logs for a deployed function
```bash
sls logs --function <functionName> --tail
```

---

## Removing Resources

### Remove the service and all associated resources

# This will remove all resources associated with the service, including functions, endpoints, and resources.So be careful when using this command.
```bash
sls remove
```

---

## Other Useful Commands

### Package the service (without deployment)
```bash
sls package
```

### Generate a CloudFormation template (without deployment)
```bash
sls package --noDeploy
```

### Check deployed endpoints and functions
```bash
sls info
```

### Check service status (functions and resources)
```bash
sls status
```

### Run serverless offline for local development
```bash
sls offline start
```

### Run serverless offline with a specific port
```bash
sls offline start --port <port>
```

### Run serverless offline with a specific host
```bash
sls offline start --host <host>
```

### Run serverless offline with a specific port and host
```bash
sls offline start --port <port> --host <host>
```

---

## Plugin Management

### Install a plugin
```bash
sls plugin install --name <pluginName>
```

### Uninstall a plugin
```bash
sls plugin uninstall --name <pluginName>
```

### List installed plugins
```bash
sls plugin list
```

---

## Configuration Validation

### Validate your service configuration
```bash
sls validate
```

---



## Help

### Display help for a specific command
```bash
sls <command> --help
```

