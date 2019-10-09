web3_clientVersion
返回当前客户端版本号

参数：
none

返回：
String - 当前客户端版本号

例子：
// Request
curl -X POST --data '{"jsonrpc":"2.0","method":"web3_clientVersion","params":[],"id":67}'

// Result
{
  "id":67,
  "jsonrpc":"2.0",
  "result": "Mist/v0.9.3/darwin/go1.4.1"
}
web3_sha3
返回指定数据的Keccak-256（不是标准化的SHA3-256）。

参数：
String - 将数据转化为SHA3哈希
params: [
  '0x68656c6c6f20776f726c64'
]
返回：
DATA - 返回SHA3

例子：
// Request
curl -X POST --data '{"jsonrpc":"2.0","method":"web3_sha3","params":["0x68656c6c6f20776f726c64"],"id":64}'

// Result
{
  "id":64,
  "jsonrpc": "2.0",
  "result": "0x47173285a8d7341e5e972fc677286384f802f8ef42a5ec5f03bbfa254cb01fad"
}
net_version
Returns the current network protocol version.
返回当前网络协议的版本。

参数：
none

返回：
String - 当前网络协议版本

举例：
// Request
curl -X POST --data '{"jsonrpc":"2.0","method":"net_version","params":[],"id":67}'

// Result
{
  "id":67,
  "jsonrpc": "2.0",
  "result": "59"
}
net_listening
如果客户端正在主动监听网络连接，则返回true。

参数：
none

返回：
Boolean - 当监听时为true，否则为false。

例子：
// Request
curl -X POST --data '{"jsonrpc":"2.0","method":"net_listening","params":[],"id":67}'

// Result
{
  "id":67,
  "jsonrpc":"2.0",
  "result":true
}
