[![Sourcegraph](https://sourcegraph.com/github.com/1lann/scopedjson/-/badge.svg)](https://sourcegraph.com/github.com/1lann/scopedjson?badge)
[![GoDoc](http://img.shields.io/badge/go-documentation-blue.svg?style=flat-square)](http://godoc.org/github.com/1lann/scopedjson)
[![Build Status](https://travis-ci.org/json-iterator/go.svg?branch=master)](https://travis-ci.org/json-iterator/go)
[![codecov](https://codecov.io/gh/json-iterator/go/branch/master/graph/badge.svg)](https://codecov.io/gh/json-iterator/go)
[![rcard](https://goreportcard.com/badge/github.com/1lann/scopedjson)](https://goreportcard.com/report/github.com/1lann/scopedjson)
[![License](http://img.shields.io/badge/license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/json-iterator/go/master/LICENSE)
[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/json-iterator/Lobby)

A high-performance 100% compatible drop-in replacement of "encoding/json"

You can also use thrift like JSON using [thrift-iterator](https://github.com/thrift-iterator/go)

# Usage

100% compatibility with standard lib

Replace

```go
import "encoding/json"
json.Marshal(&data)
```

with

```go
import jsoniter "github.com/1lann/scopedjson"

var json = jsoniter.ConfigCompatibleWithStandardLibrary
json.Marshal(&data)
```

Replace

```go
import "encoding/json"
json.Unmarshal(input, &data)
```

with

```go
import jsoniter "github.com/1lann/scopedjson"

var json = jsoniter.ConfigCompatibleWithStandardLibrary
json.Unmarshal(input, &data)
```

[More documentation](http://jsoniter.com/migrate-from-go-std.html)

# How to get

```
go get github.com/1lann/scopedjson
```

# Contribution Welcomed !

Contributors

* [thockin](https://github.com/thockin)
* [mattn](https://github.com/mattn)
* [cch123](https://github.com/cch123)
* [Oleg Shaldybin](https://github.com/olegshaldybin)
* [Jason Toffaletti](https://github.com/toffaletti)

Report issue or pull request, or email taowen@gmail.com, or [![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/json-iterator/Lobby)
