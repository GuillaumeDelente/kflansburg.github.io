---
title: "Creating an IPv6 CNI Driver in Rust"
date: 2020-11-29T08:54:27-07:00
draft: true
tags:

- Rust
- Kubernetes
- CNI
- IPv6

---

A [recent post on HackerNews](https://news.ycombinator.com/item?id=25245057) by
user [jmillikin](https://news.ycombinator.com/user?id=jmillikin) described a
technique for configuring IPv6 Kubernetes Pod addresses while remaining
compatible with an IPv4 network fabric. Given my lack of familiarity with the
specifics of CNI drivers and IPv6, I decided that this would be an interesting
project to implement and document.

<!--more-->

[Kubernetes Networking: How to Write Your Own CNI Plug-in with Bash - Altoros Blog](https://www.altoros.com/blog/kubernetes-networking-writing-your-own-simple-cni-plug-in-with-bash/)
