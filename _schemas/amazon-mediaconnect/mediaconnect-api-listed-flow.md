---
description: Provides a summary of a flow, including its ARN, Availability Zone, and source type.
layout: schema
name: ListedFlow
properties_list:
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: SourceType
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Maintenance
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-listed-flow-schema.json
slug: mediaconnect-api-listed-flow
source_filename: mediaconnect-api-listed-flow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-listed-flow-schema.json\",\n  \"title\": \"ListedFlow\",\n  \"description\": \"Provides a summary of a flow, including its ARN, Availability Zone, and source type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availabilityZone\"\n          },\n          \"description\": \"The Availability Zone that the flow was created in.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"A description\
  \ of the flow.\"\n        }\n      ]\n    },\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The ARN of the flow.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the flow.\"\n        }\n      ]\n    },\n    \"SourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceType\"\n          },\n          \"description\": \"The type of source. This value is either owned (originated somewhere other than an AWS Elemental MediaConnect flow owned by another AWS account) or entitled (originated\
  \ at an AWS Elemental MediaConnect flow owned by another AWS account).\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"The current status of the flow.\"\n        }\n      ]\n    },\n    \"Maintenance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Maintenance\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenance\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Status\",\n    \"Description\",\n    \"SourceType\",\n    \"AvailabilityZone\",\n    \"FlowArn\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-listed-flow-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: ListedFlow
---
