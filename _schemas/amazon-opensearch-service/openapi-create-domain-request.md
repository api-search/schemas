---
description: CreateDomainRequest schema from Amazon OpenSearch Service
layout: schema
name: CreateDomainRequest
properties_list:
- description: Name of the OpenSearch domain to create
  name: DomainName
  type: string
- description: Version of OpenSearch or Elasticsearch
  name: EngineVersion
  type: string
- description: Container for the cluster configuration
  name: ClusterConfig
  type: object
- description: Container for EBS-based storage options
  name: EBSOptions
  type: object
- description: IAM access policy as a JSON-formatted string
  name: AccessPolicies
  type: string
provider_name: Amazon OpenSearch Service
provider_slug: amazon-opensearch-service
schema_file: json-schema/openapi-create-domain-request-schema.json
slug: openapi-create-domain-request
source_filename: openapi-create-domain-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch-service/refs/heads/main/json-schema/openapi-create-domain-request-schema.json\",\n  \"title\": \"CreateDomainRequest\",\n  \"description\": \"CreateDomainRequest schema from Amazon OpenSearch Service\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the OpenSearch domain to create\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of OpenSearch or Elasticsearch\"\n    },\n    \"ClusterConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Container for the cluster configuration\"\n    },\n    \"EBSOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Container for EBS-based storage options\"\n    },\n    \"AccessPolicies\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"IAM access policy as a JSON-formatted string\"\n    }\n  },\n  \"required\": [\n    \"DomainName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch-service/refs/heads/main/json-schema/openapi-create-domain-request-schema.json
tags:
- Analytics
- Elasticsearch
- Full-Text Search
- Log Analytics
- OpenSearch
- Search
title: CreateDomainRequest
---
