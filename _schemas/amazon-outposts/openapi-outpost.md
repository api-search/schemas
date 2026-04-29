---
description: Information about an Outpost.
layout: schema
name: Outpost
properties_list:
- description: ''
  name: OutpostId
  type: object
- description: ''
  name: OwnerId
  type: object
- description: ''
  name: OutpostArn
  type: object
- description: ''
  name: SiteId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: LifeCycleStatus
  type: object
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: AvailabilityZoneId
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: SiteArn
  type: object
- description: ''
  name: SupportedHardwareType
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-outpost-schema.json
slug: openapi-outpost
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-outpost-schema.json\",\n  \"title\": \"Outpost\",\n  \"description\": \"Information about an Outpost.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutpostId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutpostId\"\n        },\n        {\n          \"description\": \" The ID of the Outpost. \"\n        }\n      ]\n    },\n    \"OwnerId\": {\n      \"$ref\": \"#/components/schemas/OwnerId\"\n    },\n    \"OutpostArn\": {\n      \"$ref\": \"#/components/schemas/OutpostArn\"\n    },\n    \"SiteId\": {\n      \"$ref\": \"#/components/schemas/SiteId\"\n    },\n    \"Name\": {\n      \"$ref\": \"#/components/schemas/OutpostName\"\n    },\n    \"Description\": {\n      \"$ref\": \"#/components/schemas/OutpostDescription\"\n    },\n    \"LifeCycleStatus\": {\n\
  \      \"$ref\": \"#/components/schemas/LifeCycleStatus\"\n    },\n    \"AvailabilityZone\": {\n      \"$ref\": \"#/components/schemas/AvailabilityZone\"\n    },\n    \"AvailabilityZoneId\": {\n      \"$ref\": \"#/components/schemas/AvailabilityZoneId\"\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The Outpost tags.\"\n        }\n      ]\n    },\n    \"SiteArn\": {\n      \"$ref\": \"#/components/schemas/SiteArn\"\n    },\n    \"SupportedHardwareType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SupportedHardwareType\"\n        },\n        {\n          \"description\": \" The hardware type. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-outpost-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: Outpost
---
