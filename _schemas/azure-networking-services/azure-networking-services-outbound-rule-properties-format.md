---
description: Outbound rule of the load balancer.
layout: schema
name: OutboundRulePropertiesFormat
properties_list:
- description: The number of outbound ports to be used for NAT.
  name: allocatedOutboundPorts
  type: integer
- description: Reference to another subresource.
  name: backendAddressPool
  type: object
- description: Receive bidirectional TCP Reset on TCP flow idle timeout or unexpected connection termination. This element is only used when the protocol is set to TCP.
  name: enableTcpReset
  type: boolean
- description: The Frontend IP addresses of the load balancer.
  name: frontendIPConfigurations
  type: array
- description: The timeout for the TCP idle connection.
  name: idleTimeoutInMinutes
  type: integer
- description: The protocol for the outbound rule in load balancer.
  name: protocol
  type: string
- description: The current provisioning state.
  name: provisioningState
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-outbound-rule-properties-format-schema.json
slug: azure-networking-services-outbound-rule-properties-format
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: OutboundRulePropertiesFormat
---
