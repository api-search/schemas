---
description: Request body for provisioning an infrastructure resource
layout: schema
name: ProvisionResourceRequest
properties_list:
- description: Type of infrastructure resource to provision
  name: resource_type
  type: string
- description: Name for the infrastructure resource
  name: name
  type: string
- description: Namespace the resource will be associated with
  name: namespace
  type: string
- description: Resource-specific configuration parameters
  name: configuration
  type: object
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schema_file: json-schema/platform-services-provision-resource-request-schema.json
slug: platform-services-provision-resource-request
source_filename: platform-services-provision-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-provision-resource-request-schema.json\",\n  \"title\": \"ProvisionResourceRequest\",\n  \"description\": \"Request body for provisioning an infrastructure resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resource_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of infrastructure resource to provision\",\n      \"enum\": [\n        \"redis\",\n        \"rds\",\n        \"msk\",\n        \"s3\"\n      ],\n      \"example\": \"redis\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the infrastructure resource\",\n      \"example\": \"policy-cache\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Namespace the resource will be associated with\",\n      \"example\"\
  : \"insurance-policy\"\n    },\n    \"configuration\": {\n      \"type\": \"object\",\n      \"description\": \"Resource-specific configuration parameters\",\n      \"example\": {\n        \"instance_type\": \"cache.t3.medium\",\n        \"engine_version\": \"7.0\"\n      }\n    }\n  },\n  \"required\": [\n    \"resource_type\",\n    \"name\",\n    \"namespace\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-provision-resource-request-schema.json
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
title: ProvisionResourceRequest
---
