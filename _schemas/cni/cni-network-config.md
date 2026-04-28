---
description: Schema for the Container Network Interface (CNI) network configuration document. This JSON object is passed to a CNI plugin via stdin when the container runtime invokes the plugin to attach (ADD), detach (DEL), or check (CHECK) a container's network interface. The configuration specifies the plugin type, IPAM settings, capabilities, and plugin-specific parameters.
layout: schema
name: CNI Network Configuration
properties_list:
- description: The version of the CNI specification this configuration conforms to.
  name: cniVersion
  type: string
- description: List of CNI specification versions this plugin supports, used in VERSION responses.
  name: cniVersions
  type: array
- description: Network name. Must be unique across all network configurations on a host. Used to identify the network when multiple configurations exist.
  name: name
  type: string
- description: Name of the CNI plugin binary to invoke. The container runtime will search for an executable with this name in the configured plugin search path.
  name: type
  type: string
- description: Optional additional arguments provided by the container runtime. The CNI_ARGS environment variable supersedes this field when both are set.
  name: args
  type: object
- description: If true, the plugin should configure IP masquerade (NAT) on the host for traffic leaving the network.
  name: ipMasq
  type: boolean
- description: ''
  name: ipam
  type: object
- description: ''
  name: dns
  type: object
- description: Map of capability names to boolean values indicating which runtime capabilities this plugin supports. Used by the runtime to determine which well-known fields to pass in runtimeConfig.
  name: capabilities
  type: object
- description: Runtime-injected configuration values corresponding to the declared capabilities. Populated by the container runtime with per-attachment values such as port mappings.
  name: runtimeConfig
  type: object
- description: ''
  name: prevResult
  type: object
provider_name: Container Network Interface (CNI)
provider_slug: cni
schema_file: json-schema/cni-network-config-schema.json
slug: cni-network-config
tags:
- Cloud Native
- Containers
- Incubating
- Kubernetes
- Networking
- Plugins
title: CNI Network Configuration
---
