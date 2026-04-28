---
description: Schema for the Container Network Interface (CNI) plugin result document returned on stdout after a successful ADD or CHECK operation. The result reports the network interfaces created, IP addresses assigned, routes configured, and DNS settings applied in the container network namespace. This document is also passed as the prevResult field when chaining multiple CNI plugins together.
layout: schema
name: CNI Plugin Result
properties_list:
- description: The CNI specification version this result conforms to. Should match the cniVersion from the network configuration.
  name: cniVersion
  type: string
- description: List of network interfaces created or configured during the ADD operation. Index 0 is typically the host-side veth, index 1 is the container-side interface.
  name: interfaces
  type: array
- description: List of IP addresses assigned to the container's network interfaces by the IPAM plugin.
  name: ips
  type: array
- description: List of routes that were added to the container network namespace.
  name: routes
  type: array
- description: ''
  name: dns
  type: object
provider_name: Container Network Interface (CNI)
provider_slug: cni
schema_file: json-schema/cni-result-schema.json
slug: cni-result
tags:
- Cloud Native
- Containers
- Incubating
- Kubernetes
- Networking
- Plugins
title: CNI Plugin Result
---
