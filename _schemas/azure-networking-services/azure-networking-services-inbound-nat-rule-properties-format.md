---
description: Properties of the inbound NAT rule.
layout: schema
name: InboundNatRulePropertiesFormat
properties_list:
- description: A reference to a private IP address defined on a network interface of a VM. Traffic sent to the frontend port of each of the frontend IP configurations is forwarded to the backend IP.
  name: backendIPConfiguration
  type: object
- description: The port used for the internal endpoint. Acceptable values range from 1 to 65535.
  name: backendPort
  type: integer
- description: Configures a virtual machine's endpoint for the floating IP capability required to configure a SQL AlwaysOn Availability Group. This setting is required when using the SQL AlwaysOn Availability Groups
  name: enableFloatingIP
  type: boolean
- description: Receive bidirectional TCP Reset on TCP flow idle timeout or unexpected connection termination. This element is only used when the protocol is set to TCP.
  name: enableTcpReset
  type: boolean
- description: Reference to another subresource.
  name: frontendIPConfiguration
  type: object
- description: The port for the external endpoint. Port numbers for each rule must be unique within the Load Balancer. Acceptable values range from 1 to 65534.
  name: frontendPort
  type: integer
- description: The timeout for the TCP idle connection. The value can be set between 4 and 30 minutes. The default value is 4 minutes. This element is only used when the protocol is set to TCP.
  name: idleTimeoutInMinutes
  type: integer
- description: The transport protocol for the endpoint.
  name: protocol
  type: string
- description: The current provisioning state.
  name: provisioningState
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-inbound-nat-rule-properties-format-schema.json
slug: azure-networking-services-inbound-nat-rule-properties-format
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: InboundNatRulePropertiesFormat
---
