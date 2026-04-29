---
description: v1PortStatus schema from Argo CD API
layout: schema
name: v1PortStatus
properties_list:
- description: ''
  name: error
  type: string
- description: ''
  name: port
  type: integer
- description: ''
  name: protocol
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-port-status-schema.json
slug: argo-cd-v1-port-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-port-status-schema.json\",\n  \"title\": \"v1PortStatus\",\n  \"description\": \"v1PortStatus schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"title\": \"Error is to record the problem with the service port\\nThe format of the error shall comply with the following rules:\\n- built-in error values shall be specified in this file and those shall use\\n  CamelCase names\\n- cloud provider specific error values must have names that comply with the\\n  format foo.example.com/CamelCase.\\n---\\nThe regex it matches is (dns1123SubdomainFmt/)?(qualifiedNameFmt)\\n+optional\\n+kubebuilder:validation:Required\\n+kubebuilder:validation:Pattern=`^([a-z0-9]([-a-z0-9]*[a-z0-9])?(\\\\.[a-z0-9]([-a-z0-9]*[a-z0-9])?)*/)?(([A-Za-z0-9][-A-Za-z0-9_.]*)?[A-Za-z0-9])$`\\\
  n+kubebuilder:validation:MaxLength=316\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"title\": \"Port is the port number of the service port of which status is recorded here\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"title\": \"Protocol is the protocol of the service port of which status is recorded here\\nThe supported values are: \\\"TCP\\\", \\\"UDP\\\", \\\"SCTP\\\"\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-port-status-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1PortStatus
---
