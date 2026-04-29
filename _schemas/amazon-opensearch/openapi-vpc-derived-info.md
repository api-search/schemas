---
description: Options to specify the subnets and security groups for VPC endpoint. For more information, see <a href="http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-vpc.html" target="_blank"> VPC Endpoints for Amazon Elasticsearch Service Domains</a>.
layout: schema
name: VPCDerivedInfo
properties_list:
- description: ''
  name: VPCId
  type: object
- description: ''
  name: SubnetIds
  type: object
- description: ''
  name: AvailabilityZones
  type: object
- description: ''
  name: SecurityGroupIds
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-vpc-derived-info-schema.json
slug: openapi-vpc-derived-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-vpc-derived-info-schema.json\",\n  \"title\": \"VPCDerivedInfo\",\n  \"description\": \"Options to specify the subnets and security groups for VPC endpoint. For more information, see <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-vpc.html\\\" target=\\\"_blank\\\"> VPC Endpoints for Amazon Elasticsearch Service Domains</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VPCId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The VPC Id for the Elasticsearch domain. Exists only if the domain was created with VPCOptions.\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\
  \n        },\n        {\n          \"description\": \"Specifies the subnets for VPC endpoint.\"\n        }\n      ]\n    },\n    \"AvailabilityZones\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"The availability zones for the Elasticsearch domain. Exists only if the domain was created with VPCOptions.\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"Specifies the security groups for VPC endpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-vpc-derived-info-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: VPCDerivedInfo
---
