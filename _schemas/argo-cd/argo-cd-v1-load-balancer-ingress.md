---
description: 'LoadBalancerIngress represents the status of a load-balancer ingress point: traffic intended for the service should be sent to an ingress point.'
layout: schema
name: v1LoadBalancerIngress
properties_list:
- description: ''
  name: hostname
  type: string
- description: ''
  name: ip
  type: string
- description: ''
  name: ipMode
  type: string
- description: ''
  name: ports
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-load-balancer-ingress-schema.json
slug: argo-cd-v1-load-balancer-ingress
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-load-balancer-ingress-schema.json\",\n  \"title\": \"v1LoadBalancerIngress\",\n  \"description\": \"LoadBalancerIngress represents the status of a load-balancer ingress point:\\ntraffic intended for the service should be sent to an ingress point.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hostname\": {\n      \"type\": \"string\",\n      \"title\": \"Hostname is set for load-balancer ingress points that are DNS based\\n(typically AWS load-balancers)\\n+optional\"\n    },\n    \"ip\": {\n      \"type\": \"string\",\n      \"title\": \"IP is set for load-balancer ingress points that are IP based\\n(typically GCE or OpenStack load-balancers)\\n+optional\"\n    },\n    \"ipMode\": {\n      \"type\": \"string\",\n      \"title\": \"IPMode specifies how the load-balancer IP behaves, and may only\
  \ be specified when the ip field is specified.\\nSetting this to \\\"VIP\\\" indicates that traffic is delivered to the node with\\nthe destination set to the load-balancer's IP and port.\\nSetting this to \\\"Proxy\\\" indicates that traffic is delivered to the node or pod with\\nthe destination set to the node's IP and node port or the pod's IP and port.\\nService implementations may use this information to adjust traffic routing.\\n+optional\"\n    },\n    \"ports\": {\n      \"type\": \"array\",\n      \"title\": \"Ports is a list of records of service ports\\nIf used, every port defined in the service should have an entry in it\\n+listType=atomic\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1PortStatus\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-load-balancer-ingress-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1LoadBalancerIngress
---
