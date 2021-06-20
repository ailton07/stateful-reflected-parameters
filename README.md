## README
[TODO]

This project is a fork of reflected-parameters project designed to be a stateful version.


# Build

To build, execute the following commands in project directory
```
$ gradle clean
$ gradle fatJar
```

The Jar is created under the $project/build/libs/ folder.
For more information about the build: [link](https://mkyong.com/gradle/gradle-create-a-jar-file-with-dependencies/)


# How does it work?

1. Analyze In Scope Http responses, registering the returned json values in memory (but, process only responses from Proxy).
2. Look for refections in the following In Scope HttpRequests
   * Here, we consider values in header and body.


You can use the following API for test purpose: https://repl.it/@Ailtonda/RESTserver#index.js
* Producer: https://restserver.ailtonda.repl.co/
* Consumer: https://restserver.ailtonda.repl.co/id123?id=id123
