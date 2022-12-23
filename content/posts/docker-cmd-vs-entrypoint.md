---
title: "Dockerfile CMD vs ENTRYPOINT"
date: 2022-12-23T10:31:07+05:30
draft: false
categories: [ virtualization ]
tags: [docker, dockerfile, k8s, containers]
---

## Introduction

`ENTRYPOINT` is the command that is run
`CMD` is the parameter passed to the command.


```dockerfile
FROM ubuntu
ENTRYPOINT ["sleep"]
CMD ["5m"]
```
For example in this case we are overriding the default command of ubuntu docker image with `sleep` command and the default parameters for that command is `5m`.