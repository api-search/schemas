---
description: Properties of the load balancer.
layout: schema
name: LoadBalancingRulePropertiesFormat
properties_list:
- description: Reference to another subresource.
  name: backendAddressPool
  type: object
- description: The port used for internal connections on the endpoint. Acceptable values are between 0 and 65535. Note that value 0 enables "Any Port".
  name: backendPort
  type: integer
- description: Configures SNAT for the VMs in the backend pool to use the publicIP address specified in the frontend of the load balancing rule.
  name: disableOutboundSnat
  type: boolean
- description: Configures a virtual machine's endpoint for the floating IP capability required to configure a SQL AlwaysOn Availability Group. This setting is required when using the SQL AlwaysOn Availability Groups
  name: enableFloatingIP
  type: boolean
- description: Receive bidirectional TCP Reset on TCP flow idle timeout or unexpected connection termination. This element is only used when the protocol is set to TCP.
  name: enableTcpReset
  type: boolean
- description: Reference to another subresource.
  name: frontendIPConfiguration
  type: object
- description: The port for the external endpoint. Port numbers for each rule must be unique within the Load Balancer. Acceptable values are between 0 and 65534. Note that value 0 enables "Any Port".
  name: frontendPort
  type: integer
- description: The timeout for the TCP idle connection. The value can be set between 4 and 30 minutes. The default value is 4 minutes. This element is only used when the protocol is set to TCP.
  name: idleTimeoutInMinutes
  type: integer
- description: The load distribution policy for this rule.
  name: loadDistribution
  type: string
- description: Reference to another subresource.
  name: probe
  type: object
- description: The reference to the transport protocol used by the load balancing rule.
  name: protocol
  type: object
- description: The current provisioning state.
  name: provisioningState
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-load-balancing-rule-properties-format-schema.json
slug: azure-networking-services-load-balancing-rule-properties-format
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: LoadBalancingRulePropertiesFormat
---
