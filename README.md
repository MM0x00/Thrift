# Thrift 在线实验环境

## 软件简介

Apache Thrift软件框架用于可扩展的跨语言服务开发，将软件堆栈与代码生成引擎相结合，构建可在C ++，Java，Python，PHP，Ruby，Erlang，Perl，Haskell，C＃之间高效无缝工作的服务， Cocoa，JavaScript，Node.js，Smalltalk，OCaml和Delphi等语言。

所属类别是web开发

LicenseAPACHE LICENSE, VERSION 2.0 

特点:

支持语言种类多

## 软件官网

https://thrift.apache.org/

## Dockerfile 使用方法

### 如何使用
旨在作为可执行文件运行。通过安装目录提供文件。这是一个service.thrift将ruby 编译到当前目录的示例。
```
$ docker run -v "$PWD:/data" thrift thrift -o /data --gen rb /data/service.thrift
```
请注意，您可能希望包括-u $(id -u)在生成的文件上设置UID。休眠过程默认以root身份运行，这将根据您的docker设置生成根拥有的文件。

## 资源链接

- https://thrift.apache.org/
