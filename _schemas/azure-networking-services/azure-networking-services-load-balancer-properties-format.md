---
description: Properties of the load balancer.
layout: schema
name: LoadBalancerPropertiesFormat
properties_list:
- description: Collection of backend address pools used by a load balancer.
  name: backendAddressPools
  type: array
- description: Object representing the frontend IPs to be used for the load balancer.
  name: frontendIPConfigurations
  type: array
- description: Defines an external port range for inbound NAT to a single backend port on NICs associated with a load balancer. Inbound NAT rules are created automatically for each NIC associated with the Load Balan
  name: inboundNatPools
  type: array
- description: Collection of inbound NAT Rules used by a load balancer. Defining inbound NAT rules on your load balancer is mutually exclusive with defining an inbound NAT pool. Inbound NAT pools are referenced from
  name: inboundNatRules
  type: array
- description: Object collection representing the load balancing rules Gets the provisioning.
  name: loadBalancingRules
  type: array
- description: The outbound rules.
  name: outboundRules
  type: array
- description: Collection of probe objects used in the load balancer.
  name: probes
  type: array
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: The resource GUID property of the load balancer resource.
  name: resourceGuid
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-load-balancer-properties-format-schema.json
slug: azure-networking-services-load-balancer-properties-format
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: LoadBalancerPropertiesFormat
---
