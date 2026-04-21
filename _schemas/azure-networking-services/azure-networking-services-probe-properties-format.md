---
description: Load balancer probe resource.
layout: schema
name: ProbePropertiesFormat
properties_list:
- description: The interval, in seconds, for how frequently to probe the endpoint for health status. Typically, the interval is slightly less than half the allocated timeout period (in seconds) which allows two full
  name: intervalInSeconds
  type: integer
- description: The load balancer rules that use this probe.
  name: loadBalancingRules
  type: array
- description: 'The number of probes where if no response, will result in stopping further traffic from being delivered to the endpoint. This values allows endpoints to be taken out of rotation faster or slower than '
  name: numberOfProbes
  type: integer
- description: The port for communicating the probe. Possible values range from 1 to 65535, inclusive.
  name: port
  type: integer
- description: The protocol of the end point. If 'Tcp' is specified, a received ACK is required for the probe to be successful. If 'Http' or 'Https' is specified, a 200 OK response from the specifies URI is required
  name: protocol
  type: string
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: The URI used for requesting health status from the VM. Path is required if a protocol is set to http. Otherwise, it is not allowed. There is no default value.
  name: requestPath
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-probe-properties-format-schema.json
slug: azure-networking-services-probe-properties-format
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: ProbePropertiesFormat
---
