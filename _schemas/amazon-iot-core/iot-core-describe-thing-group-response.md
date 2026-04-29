---
description: DescribeThingGroupResponse schema
layout: schema
name: DescribeThingGroupResponse
properties_list:
- description: ''
  name: thingGroupName
  type: object
- description: ''
  name: thingGroupId
  type: object
- description: ''
  name: thingGroupArn
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: thingGroupProperties
  type: object
- description: ''
  name: thingGroupMetadata
  type: object
- description: ''
  name: indexName
  type: object
- description: ''
  name: queryString
  type: object
- description: ''
  name: queryVersion
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-describe-thing-group-response-schema.json
slug: iot-core-describe-thing-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-thing-group-response-schema.json\",\n  \"title\": \"DescribeThingGroupResponse\",\n  \"description\": \"DescribeThingGroupResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupName\"\n        },\n        {\n          \"description\": \"The name of the thing group.\"\n        }\n      ]\n    },\n    \"thingGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupId\"\n        },\n        {\n          \"description\": \"The thing group ID.\"\n        }\n      ]\n    },\n    \"thingGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupArn\"\n        },\n        {\n          \"description\"\
  : \"The thing group ARN.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the thing group.\"\n        }\n      ]\n    },\n    \"thingGroupProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupProperties\"\n        },\n        {\n          \"description\": \"The thing group properties.\"\n        }\n      ]\n    },\n    \"thingGroupMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupMetadata\"\n        },\n        {\n          \"description\": \"Thing group metadata.\"\n        }\n      ]\n    },\n    \"indexName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IndexName\"\n        },\n        {\n          \"description\": \"The dynamic thing group index name.\"\n        }\n      ]\n    },\n    \"queryString\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryString\"\n        },\n        {\n          \"description\": \"The dynamic thing group search query string.\"\n        }\n      ]\n    },\n    \"queryVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryVersion\"\n        },\n        {\n          \"description\": \"The dynamic thing group query version.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DynamicGroupStatus\"\n        },\n        {\n          \"description\": \"The dynamic thing group status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-thing-group-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: DescribeThingGroupResponse
---
