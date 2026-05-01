---
description: DescribeIndexResponse schema
layout: schema
name: DescribeIndexResponse
properties_list:
- description: ''
  name: indexName
  type: object
- description: ''
  name: indexStatus
  type: object
- description: ''
  name: schema
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-index-response-schema.json
slug: iot-device-management-describe-index-response
source_filename: iot-device-management-describe-index-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-index-response-schema.json\",\n  \"title\": \"DescribeIndexResponse\",\n  \"description\": \"DescribeIndexResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"indexName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IndexName\"\n        },\n        {\n          \"description\": \"The index name.\"\n        }\n      ]\n    },\n    \"indexStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IndexStatus\"\n        },\n        {\n          \"description\": \"The index status.\"\n        }\n      ]\n    },\n    \"schema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IndexSchema\"\n        },\n        {\n          \"description\": \"<p>Contains a value\
  \ that specifies the type of indexing performed. Valid values are:</p> <ul> <li> <p>REGISTRY \\u2013 Your thing index contains only registry data.</p> </li> <li> <p>REGISTRY_AND_SHADOW - Your thing index contains registry data and shadow data.</p> </li> <li> <p>REGISTRY_AND_CONNECTIVITY_STATUS - Your thing index contains registry data and thing connectivity status data.</p> </li> <li> <p>REGISTRY_AND_SHADOW_AND_CONNECTIVITY_STATUS - Your thing index contains registry data, shadow data, and thing connectivity status data.</p> </li> <li> <p>MULTI_INDEXING_MODE - Your thing index contains multiple data sources. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot/latest/apireference/API_GetIndexingConfiguration.html\\\">GetIndexingConfiguration</a>.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-index-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeIndexResponse
---
