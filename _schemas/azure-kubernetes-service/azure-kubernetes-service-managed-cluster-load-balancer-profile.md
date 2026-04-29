---
description: Profile of the managed cluster load balancer.
layout: schema
name: ManagedClusterLoadBalancerProfile
properties_list:
- description: Desired managed outbound IPs for the cluster load balancer.
  name: managedOutboundIPs
  type: object
- description: Desired outbound IP Prefix resources for the cluster load balancer.
  name: outboundIPPrefixes
  type: object
- description: Desired outbound IP resources for the cluster load balancer.
  name: outboundIPs
  type: object
- description: The effective outbound IP resources of the cluster load balancer.
  name: effectiveOutboundIPs
  type: array
- description: The desired number of allocated SNAT ports per VM.
  name: allocatedOutboundPorts
  type: integer
- description: Desired outbound flow idle timeout in minutes.
  name: idleTimeoutInMinutes
  type: integer
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-load-balancer-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-load-balancer-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterLoadBalancerProfile\",\n  \"type\": \"object\",\n  \"description\": \"Profile of the managed cluster load balancer.\",\n  \"properties\": {\n    \"managedOutboundIPs\": {\n      \"type\": \"object\",\n      \"description\": \"Desired managed outbound IPs for the cluster load balancer.\"\n    },\n    \"outboundIPPrefixes\": {\n      \"type\": \"object\",\n      \"description\": \"Desired outbound IP Prefix resources for the cluster load balancer.\"\n    },\n    \"outboundIPs\": {\n      \"type\": \"object\",\n      \"description\": \"Desired outbound IP resources for the cluster load balancer.\"\n    },\n    \"effectiveOutboundIPs\": {\n      \"type\": \"array\",\n      \"description\": \"The effective outbound IP resources of the cluster load balancer.\"\n    },\n    \"allocatedOutboundPorts\": {\n      \"type\": \"integer\",\n      \"description\": \"The desired number of allocated\
  \ SNAT ports per VM.\"\n    },\n    \"idleTimeoutInMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Desired outbound flow idle timeout in minutes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-load-balancer-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterLoadBalancerProfile
---
