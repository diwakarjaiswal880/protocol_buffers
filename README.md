# Protocol Buffer
# The Protocol Buffer Data Format
Protocol buffers, are essentially a data format, much like JSON or XML in the sense that they store structured data which can be serialized or de-serialized by a wide number of different languages.

The main advantage of this format is that it’s a hell of a lot smaller when compared to the likes of XML or even JSON. It was a format that was originally developed by Google, who are fairly well known company that are at such a size, that every byte they can save makes a difference.

This will download the necessary packages
$ go get github.com/golang/protobuf
$ go get github.com/golang/protobuf/proto

set path
$ export PATH=$PATH:$GOPATH/bin

compile proto file
$ protoc --go_out=. *.proto


When we run this, we need to ensure that we pass in our 'test.pb.go' file as well in order for this to work:
$ go run main.go test.pb.go
