---
description: Options to specify the subnets and security groups for VPC endpoint. For more information, see <a href="http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-vpc.html" target="_blank"> VPC Endpoints for Amazon Elasticsearch Service Domains</a>.
layout: schema
name: VPCOptions
properties_list:
- description: ''
  name: SubnetIds
  type: object
- description: ''
  name: SecurityGroupIds
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-vpc-options-schema.json
slug: openapi-vpc-options
source_filename: openapi-vpc-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-vpc-options-schema.json\",\n  \"title\": \"VPCOptions\",\n  \"description\": \"Options to specify the subnets and security groups for VPC endpoint. For more information, see <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-vpc.html\\\" target=\\\"_blank\\\"> VPC Endpoints for Amazon Elasticsearch Service Domains</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"Specifies the subnets for VPC endpoint.\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\"\
  : \"Specifies the security groups for VPC endpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-vpc-options-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: VPCOptions
---
