## 環境構築
- Go をインストール
```
$ brew install go
```

- 環境変数を追記
```.bashrc
export GOROOT=/usr/local/opt/go/libexec
export GOPATH=$HOME # 作業ディレクトリ
export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
```

- protoc をインストール
```
$ brew install protoc
```

- protoc Go plugin をインストール
```
$ go get -u github.com/golang/protobuf/protoc-gen-go
```

## Golangで自分自身で定義したパッケージをインポートする方法
- github へ pushする
- go get
```
$ go get github.com/kawabatas/go-grpc-sample/protocol
```

## 参考
https://qiita.com/h3_poteto/items/3a39c41743b4fd87c134
