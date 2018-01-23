Documentation for the JSON-RPC implementation

# Links

* http://www.jsonrpc.org/specification
* https://github.com/neo-project/neo/blob/master/neo/Network/RPC/RpcServer.cs
* http://docs.neo.org/en-us/node/api.html


# JSON-RPC API Calls

## `getaccountstate`

### with invalid address

Request:

    curl -X POST -H "Content-Type: application/json" -d '{"jsonrpc": "2.0","method": "getaccountstate","params": ["Axozf8x8GmyLnNv8ikQcPKgRHQTbFi46u2"],"id": 1}' https://seed1.neo.org:20331

neo-cli response:

    {"jsonrpc":"2.0","id":1,"error":{"code":-2146233033,"message":"One of the identified items was in an invalid format."}
