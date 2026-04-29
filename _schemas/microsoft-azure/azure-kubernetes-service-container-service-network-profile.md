---
description: Profile of network configuration.
layout: schema
name: ContainerServiceNetworkProfile
properties_list:
- description: Network plugin used for building the Kubernetes network.
  name: networkPlugin
  type: string
- description: The mode the network plugin should use.
  name: networkPluginMode
  type: string
- description: Network policy used for building the Kubernetes network.
  name: networkPolicy
  type: string
- description: The network dataplane used in the Kubernetes cluster.
  name: networkDataplane
  type: string
- description: A CIDR notation IP range from which to assign pod IPs.
  name: podCidr
  type: string
- description: A CIDR notation IP range from which to assign service cluster IPs.
  name: serviceCidr
  type: string
- description: An IP address assigned to the Kubernetes DNS service.
  name: dnsServiceIP
  type: string
- description: The load balancer sku for the managed cluster.
  name: loadBalancerSku
  type: string
- description: The outbound (egress) routing method.
  name: outboundType
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-kubernetes-service-container-service-network-profile-schema.json
slug: azure-kubernetes-service-container-service-network-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContainerServiceNetworkProfile\",\n  \"type\": \"object\",\n  \"description\": \"Profile of network configuration.\",\n  \"properties\": {\n    \"networkPlugin\": {\n      \"type\": \"string\",\n      \"description\": \"Network plugin used for building the Kubernetes network.\"\n    },\n    \"networkPluginMode\": {\n      \"type\": \"string\",\n      \"description\": \"The mode the network plugin should use.\"\n    },\n    \"networkPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"Network policy used for building the Kubernetes network.\"\n    },\n    \"networkDataplane\": {\n      \"type\": \"string\",\n      \"description\": \"The network dataplane used in the Kubernetes cluster.\"\n    },\n    \"podCidr\": {\n      \"type\": \"string\",\n      \"description\": \"A CIDR notation IP range from which to assign pod IPs.\"\n    },\n    \"serviceCidr\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"A CIDR notation IP range from which to assign service cluster IPs.\"\n    },\n    \"dnsServiceIP\": {\n      \"type\": \"string\",\n      \"description\": \"An IP address assigned to the Kubernetes DNS service.\"\n    },\n    \"loadBalancerSku\": {\n      \"type\": \"string\",\n      \"description\": \"The load balancer sku for the managed cluster.\"\n    },\n    \"outboundType\": {\n      \"type\": \"string\",\n      \"description\": \"The outbound (egress) routing method.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-kubernetes-service-container-service-network-profile-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ContainerServiceNetworkProfile
---
