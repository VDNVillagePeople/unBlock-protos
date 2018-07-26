# unBlock-protos

Swift
protoc --swift_out=../protos-swift *.proto

Typescript
node_modules/protobufjs/bin/pbjs -t static-module -w commonjs -o src/app/protos/compiled.js protos/*.proto
node_modules/protobufjs/bin/pbts -o src/app/protos/compiled.d.ts src/app/protos/compiled.js

Dart
protoc --dart_out=../lib/protos/ *.proto
