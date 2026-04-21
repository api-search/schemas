---
description: Properties of Inbound NAT pool.
layout: schema
name: InboundNatPoolPropertiesFormat
properties_list:
- description: The port used for internal connections on the endpoint. Acceptable values are between 1 and 65535.
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
- description: The last port number in the range of external ports that will be used to provide Inbound Nat to NICs associated with a load balancer. Acceptable values range between 1 and 65535.
  name: frontendPortRangeEnd
  type: integer
- description: The first port number in the range of external ports that will be used to provide Inbound Nat to NICs associated with a load balancer. Acceptable values range between 1 and 65534.
  name: frontendPortRangeStart
  type: integer
- description: The timeout for the TCP idle connection. The value can be set between 4 and 30 minutes. The default value is 4 minutes. This element is only used when the protocol is set to TCP.
  name: idleTimeoutInMinutes
  type: integer
- description: The reference to the transport protocol used by the inbound NAT pool.
  name: protocol
  type: object
- description: The current provisioning state.
  name: provisioningState
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-inbound-nat-pool-properties-format-schema.json
slug: azure-networking-services-inbound-nat-pool-properties-format
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: InboundNatPoolPropertiesFormat
---
