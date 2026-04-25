---
description: A Cilium-managed network endpoint representing a Kubernetes pod or container with associated security identity, IP addressing, and policy enforcement state.
layout: schema
name: Cilium Endpoint
properties_list:
- description: Numeric endpoint ID assigned by the Cilium agent.
  name: id
  type: integer
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
provider_name: Cilium
provider_slug: cilium
schema_file: json-schema/cilium-endpoint-schema.json
slug: cilium-endpoint
tags:
- Cloud Native
- eBPF
- Kubernetes
- Networking
- Security
title: Cilium Endpoint
---
