---
description: Each <code>LongTermPricingListEntry</code> object contains information about a long-term pricing type.
layout: schema
name: LongTermPricingListEntry
properties_list:
- description: ''
  name: LongTermPricingId
  type: object
- description: ''
  name: LongTermPricingEndDate
  type: object
- description: ''
  name: LongTermPricingStartDate
  type: object
- description: ''
  name: LongTermPricingType
  type: object
- description: ''
  name: CurrentActiveJob
  type: object
- description: ''
  name: ReplacementJob
  type: object
- description: ''
  name: IsLongTermPricingAutoRenew
  type: object
- description: ''
  name: LongTermPricingStatus
  type: object
- description: ''
  name: SnowballType
  type: object
- description: ''
  name: JobIds
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-long-term-pricing-list-entry-schema.json
slug: amazon-snow-family-long-term-pricing-list-entry
source_filename: amazon-snow-family-long-term-pricing-list-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-long-term-pricing-list-entry-schema.json\",\n  \"title\": \"LongTermPricingListEntry\",\n  \"description\": \"Each <code>LongTermPricingListEntry</code> object contains information about a long-term pricing type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LongTermPricingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongTermPricingId\"\n        },\n        {\n          \"description\": \"The ID of the long-term pricing type for the device.\"\n        }\n      ]\n    },\n    \"LongTermPricingEndDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The end date the long-term pricing contract.\"\n        }\n      ]\n    },\n    \"LongTermPricingStartDate\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start date of the long-term pricing contract.\"\n        }\n      ]\n    },\n    \"LongTermPricingType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongTermPricingType\"\n        },\n        {\n          \"description\": \"The type of long-term pricing that was selected for the device.\"\n        }\n      ]\n    },\n    \"CurrentActiveJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The current active jobs on the device the long-term pricing type.\"\n        }\n      ]\n    },\n    \"ReplacementJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"A new device that replaces a device that is ordered with long-term pricing.\"\
  \n        }\n      ]\n    },\n    \"IsLongTermPricingAutoRenew\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JavaBoolean\"\n        },\n        {\n          \"description\": \"If set to <code>true</code>, specifies that the current long-term pricing type for the device should be automatically renewed before the long-term pricing contract expires.\"\n        }\n      ]\n    },\n    \"LongTermPricingStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The status of the long-term pricing type.\"\n        }\n      ]\n    },\n    \"SnowballType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnowballType\"\n        },\n        {\n          \"description\": \"The type of Snow Family devices associated with this long-term pricing job.\"\n        }\n      ]\n    },\n    \"JobIds\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/LongTermPricingAssociatedJobIdList\"\n        },\n        {\n          \"description\": \"The IDs of the jobs that are associated with a long-term pricing type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-long-term-pricing-list-entry-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: LongTermPricingListEntry
---
