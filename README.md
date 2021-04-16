# Awesome wasmcloud

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of wasmcloud code and resources.

**wasmcloud** is a platform for writing portable business logic that can run anywhere from the edge to the cloud, that boasts a secure-by-default, boilerplate-free developer experience with rapid feedback loop.

### Contributing

If you would like to contribute to this list, please read the [contribution guidelines](https://github.com/stevelr/awesome-wasmcloud/blob/main/CONTRIBUTING.md)
first.

#### *If you see a package or project here that is no longer maintained or is not a good fit, please submit a pull request to improve this file. Thank you!*


### Contents

- Documentation and resources
  - [Documentation](#documentation)
  - [Tutorials](#tutorials)
  - [Community](#community)
  

- Code, tools, and examples
  - [Actors](#actors)
  - [Capability Providers](#capability-providers)
  - [Krustlet](#krustlet)
  - [Libraries](#Libraries)
  - [Tools](#tools)


<hr/>

## Documentation

- Official docs
  - [Overview and getting started](https://wasmcloud.dev/overview/)
  - [App development](https://wasmcloud.dev/app-dev/) - for application developers
  - [Platform building](https://wasmcloud.dev/platform-builder/) - for platform builders
  - [Reference](https://wasmcloud.dev/reference/)
  - [Quick reference (draft)](https://docs.google.com/presentation/d/1rdqL-eOHI9X7iiXZHLIeoCJbKirieZ1wmqrzvjZsJ94/edit#slide=id.gd0fc6481ae_0_279)
  - [Architectural decision log](https://wasmcloud.github.io/adr/)


## Tutorials

- [Interactive Katacoda tutorials](https://www.katacoda.com/wasmcloud)
  - [Developing applications with wasmcloud](https://www.katacoda.com/wasmcloud/courses/dev_apps)
  - [wasmcloud basics](https://www.katacoda.com/wasmcloud/courses/wasmcloud_basics)


## Community

- [Join the community](https://wasmcloud.dev/contact)
- [github](https://github.com/wasmcloud)


## Actors

- Examples
  - [actor-to-actor](https://github.com/wasmCloud/examples/tree/main/actor-to-actor) An example illustrating shared actor interface and actor-to-actor communication
  - [echo](https://github.com/wasmCloud/examples/tree/main/echo) An actor that returns a JSON payload describing the incoming request
  - [ecommerce](https://github.com/wasmCloud/examples/tree/main/ecommerce)
  - [extras](https://github.com/wasmCloud/examples/tree/main/extras) A sample illustrating the use of the wasmcloud:extras capability for random number, Guid, and sequence number generation.
  - [logger](https://github.com/wasmCloud/examples/tree/main/logger) A simple actor that logs every HTTP Request Method it receives to stdout
  - [subscriber](https://github.com/wasmCloud/examples/tree/main/subscriber) A simple actor that logs every message it receives to stdout
  - [wasmcloud Chat](https://github.com/wasmCloud/examples/tree/main/wasmcloud-chat) chat with multi-channel back-end


## Capability Providers


- Examples
  - [inmemory-keyvalue](https://github.com/wasmCloud/examples/tree/main/inmemory-keyvalue) A sample in-memory Key-Value Store capability provider, used by the tutorial for creating a new capability provider
  - [kvcounter](https://github.com/wasmCloud/examples/tree/main/kvcounter) An actor that uses the key-value store to increment a counter and return a value for every HTTP request it receives
  - [kvcounter-as](https://github.com/wasmCloud/examples/tree/main/kvcounter-as) The same actor as kvcounter, but written in AssemblyScript. This actor is meant to demonstrate the subtle differences between languages.
  

- Reference implementations
  - [fs](https://github.com/wasmCloud/capability-providers/tree/main/fs) file system provider
  - [http-client](https://github.com/wasmCloud/capability-providers/tree/main/http-client) http client
  - [http server](https://github.com/wasmCloud/capability-providers/tree/main/http-server) http server
  - [logging](https://github.com/wasmCloud/capability-providers/tree/main/logging)
  - [nats kv cache](https://github.com/wasmCloud/capability-providers/tree/main/nats-kvcache)
  - [nats](https://github.com/wasmCloud/capability-providers/tree/main/nats)
  - [redis-streams](https://github.com/wasmCloud/capability-providers/tree/main/redis-streams)
  - [redis](https://github.com/wasmCloud/capability-providers/tree/main/redis)
  - [redisgraph](https://github.com/wasmCloud/capability-providers/tree/main/redisgraph) - graph database provider
  - [s3](https://github.com/wasmCloud/capability-providers/tree/main/s3) blobstore provider
  - [telnet](https://github.com/wasmCloud/capability-providers/tree/main/telnet) telnet capability provider


## Krustlet

- [krustlet](https://krustlet.dev/) - Run WebAssembly workloads in your Kubernetes cluster
- [krustlet wasmcloud provider](https://github.com/wasmCloud/krustlet-wasmcloud-provider) - Kubernetes Rust Kubelet provider for wasmCloud 


## Libraries

- Actor
  - [actor-interfaces](https://github.com/wasmCloud/actor-interfaces) - Libraries used by actors to interface with different capability providers
  

- Host
  - [wasmcloud host](https://docs.rs/wasmcloud-host/) API for interacting with the host runtime (rust)
 

- Tooling
  - [provider-archive](https://github.com/wasmCloud/provider-archive) Library for PAR files - compressable TARs for managing OS/CPU-native capability provider plugins and signed claims (rust)
  - [wascap](https://github.com/wasmCloud/wascap) Embed, extract, and validate capability claims in JWTs for WebAssembly modules 
 

## Tools

- [WAPC cli](https://github.com/wapc/cli-go) WebAssembly Procedure Calls command-line interface.
- [wash](https://github.com/wasmCloud/wash) - WAsmcloud SHell - A multi-tool for various wasmcloud activities as well as an interactive REPL for a wasmcloud runtime host.
- [WIDL-validator](https://jsoverson.github.io/widl-validator/) Validate your WIDL yo.
