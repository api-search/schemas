---
description: Options to enable, disable, and specify the properties of EBS storage volumes. For more information, see <a href="http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-ebs" target="_blank"> Configuring EBS-based Storage</a>.
layout: schema
name: EBSOptions
properties_list:
- description: ''
  name: EBSEnabled
  type: object
- description: ''
  name: VolumeType
  type: object
- description: ''
  name: VolumeSize
  type: object
- description: ''
  name: Iops
  type: object
- description: ''
  name: Throughput
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-ebs-options-schema.json
slug: openapi-ebs-options
source_filename: openapi-ebs-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-ebs-options-schema.json\",\n  \"title\": \"EBSOptions\",\n  \"description\": \"Options to enable, disable, and specify the properties of EBS storage volumes. For more information, see <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-ebs\\\" target=\\\"_blank\\\"> Configuring EBS-based Storage</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EBSEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies whether EBS-based storage is enabled.\"\n        }\n      ]\n    },\n    \"VolumeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeType\"\n        },\n   \
  \     {\n          \"description\": \" Specifies the volume type for EBS-based storage.\"\n        }\n      ]\n    },\n    \"VolumeSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerClass\"\n        },\n        {\n          \"description\": \" Integer to specify the size of an EBS volume.\"\n        }\n      ]\n    },\n    \"Iops\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerClass\"\n        },\n        {\n          \"description\": \"Specifies the IOPS for Provisioned IOPS And GP3 EBS volume (SSD).\"\n        }\n      ]\n    },\n    \"Throughput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerClass\"\n        },\n        {\n          \"description\": \"Specifies the Throughput for GP3 EBS volume (SSD).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-ebs-options-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: EBSOptions
---
