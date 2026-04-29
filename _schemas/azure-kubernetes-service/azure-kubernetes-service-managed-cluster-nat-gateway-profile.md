---
description: Profile of the managed cluster NAT gateway.
layout: schema
name: ManagedClusterNATGatewayProfile
properties_list:
- description: The managed outbound IP profile of the NAT gateway.
  name: managedOutboundIPProfile
  type: object
- description: The effective outbound IP resources of the NAT gateway.
  name: effectiveOutboundIPs
  type: array
- description: Desired outbound flow idle timeout in minutes.
  name: idleTimeoutInMinutes
  type: integer
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-nat-gateway-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-nat-gateway-profile
source_filename: azure-kubernetes-service-managed-cluster-nat-gateway-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterNATGatewayProfile\",\n  \"type\": \"object\",\n  \"description\": \"Profile of the managed cluster NAT gateway.\",\n  \"properties\": {\n    \"managedOutboundIPProfile\": {\n      \"type\": \"object\",\n      \"description\": \"The managed outbound IP profile of the NAT gateway.\"\n    },\n    \"effectiveOutboundIPs\": {\n      \"type\": \"array\",\n      \"description\": \"The effective outbound IP resources of the NAT gateway.\"\n    },\n    \"idleTimeoutInMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Desired outbound flow idle timeout in minutes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-nat-gateway-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterNATGatewayProfile
---
