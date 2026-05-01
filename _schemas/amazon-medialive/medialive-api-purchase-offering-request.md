---
description: Placeholder documentation for PurchaseOfferingRequest
layout: schema
name: PurchaseOfferingRequest
properties_list:
- description: ''
  name: Count
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RenewalSettings
  type: object
- description: ''
  name: RequestId
  type: object
- description: ''
  name: Start
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-purchase-offering-request-schema.json
slug: medialive-api-purchase-offering-request
source_filename: medialive-api-purchase-offering-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-purchase-offering-request-schema.json\",\n  \"title\": \"PurchaseOfferingRequest\",\n  \"description\": \"Placeholder documentation for PurchaseOfferingRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"count\"\n          },\n          \"description\": \"Number of resources\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Name for the new reservation\"\n        }\n      ]\n    },\n    \"RenewalSettings\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RenewalSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"renewalSettings\"\n          },\n          \"description\": \"Renewal settings for the reservation\"\n        }\n      ]\n    },\n    \"RequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"requestId\"\n          },\n          \"description\": \"Unique request ID to be specified. This is needed to prevent retries from creating multiple resources.\"\n        }\n      ]\n    },\n    \"Start\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"start\"\n          },\n          \"description\": \"Requested reservation start time (UTC) in ISO-8601 format. The specified time must be between the first day of\
  \ the current month and one year from now. If no value is given, the default is now.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A collection of key-value pairs\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Count\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-purchase-offering-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: PurchaseOfferingRequest
---
