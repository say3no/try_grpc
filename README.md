# ほげ

protbufの思想は分かって、じゃあgrpcをgoでやる時はどうなるの？っていう疑問から。
まず、公式の`go tutorial for go`みたいなやつをなぞる。
といっても
```go
$GOPATH/src/google.golang.org/grpc/examples/helloworld
```
で

`go run greeter_server/main.go`
でサーバーを建てて、クライアントを
`go run greeter_client/main.go`
で建てるだけ。サーバー、クライアントは非常にシンプルで（そりゃそうか）すぐ分かる。

とは言え実際に使ってみないとわからない。ので、写経してみる。

まず`proto`。javaのオプションはコメントアウトして生成物`helloworld/helloworld.pb.go`と、
オリジナルをコピーした`helloworld/example.go`を比較するとコメントアウトとバイナリ以外は同じだった。




