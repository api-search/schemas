---
description: Provides information about the type and the names of attributes that were removed from all the endpoints that are associated with an application.
layout: schema
name: AttributesResource
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: AttributeType
  type: object
- description: ''
  name: Attributes
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-attributes-resource-schema.json
slug: amazon-pinpoint-attributes-resource
source_filename: amazon-pinpoint-attributes-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-attributes-resource-schema.json\",\n  \"title\": \"AttributesResource\",\n  \"description\": \"Provides information about the type and the names of attributes that were removed from all the endpoints that are associated with an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application.\"\n        }\n      ]\n    },\n    \"AttributeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The type of attribute or attributes that were removed from the endpoints. Valid values are:</p> <ul><li><p>endpoint-custom-attributes\
  \ - Custom attributes that describe endpoints.</p></li> <li><p>endpoint-metric-attributes - Custom metrics that your app reports to Amazon Pinpoint for endpoints.</p></li> <li><p>endpoint-user-attributes - Custom attributes that describe users.</p></li></ul>\"\n        }\n      ]\n    },\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOf__string\"\n        },\n        {\n          \"description\": \"An array that specifies the names of the attributes that were removed from the endpoints.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AttributeType\",\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-attributes-resource-schema.json
tags:
- AWS
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: AttributesResource
---
