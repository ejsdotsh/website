---
title: "reanimating my personal infrastructure"
draft: false
# image: //via.placeholder.com/640x150
# alt_text: "an image of reanimating project"
summary: "this project is to document, rebuild, and automate my personal infrastructure..."
status: active
tech_used:
  - Go
  - Python
  - Bash
  - Pulumi
  - Ansible
  - Salt
---

Reanimating my personal infrastructure...as code

My personal infrastructure has always been managed and defined, at least in part, through code. This began with Bourne
and Korn Shell, 'sed', 'AWK', and 'Perl', then 'cfengine' and 'puppet', and eventually 'ansible'. The larger part of my
personal infrastructure management has been through what is generally termed, 'click ops'. This project is about
eliminating (or at least significantly reducing) the necessity of having to 'click' in a graphical/web UI.

I decided to use [Pulumi](https://www.pulumi.com/) for provisioning, primarily so I wouldn't have to use HCL. As a
configuration language, HCL lacks features that facilitate higher levels of abstraction and reduce repetition, and I
prefer [Nickel Lang](https://nickel-lang.org/) or [CUE](https://cuelang.org) for defining configuration. It is also
subject to Hashicorp's decisions. That said, I am using [Go](https://go.dev/) as the initial language for my
Pulumi-driven infrastructure. This is to reduce the number of languages and tool-chains in the build pipeline, as well
as minimize the number of new things to learn.

The first step is importing my current DNS, compute, and storage infrastructure into Pulumi:

- [Digital Ocean](https://www.digitalocean.com/)
- [Linode](https://www.linode.com/)
- [Proxmox VE](https://www.proxmox.com/en/products/proxmox-virtual-environment/overview)
