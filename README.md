# j2cl_export_symbol_demo

0. install deps

```bash
go get bazelisk
```

1. build helloworld.js

     the code is samples from main j2cl repo, but with minor modification. ( the sayHello return a string, instead of void. so the value can be set to page elememt. check the git change for details)

```bash
bazelisk build //src/main/java/com/google/j2cl/samples/helloworld:helloworld
```

2. copy the helloworld.js to js project folder. 

```
cp bazel-bin/src/main/java/com/google/j2cl/samples/helloworld/helloworld.js .
cp bazel-bin/src/main/java/com/google/j2cl/samples/helloworld/helloworld.js.map .
```

check [j2cl_webpack_demo](https://github.com/swuecho/j2cl_webpack_demo)
