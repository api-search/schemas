---
description: ComplianceEvent from LinkedIn API
layout: schema
name: ComplianceEvent
properties_list:
- description: Unique identifier for the compliance event
  name: id
  type: string
- description: Timestamp when the event was captured
  name: capturedAt
  type: integer
- description: Timestamp when the event was processed
  name: processedAt
  type: integer
- description: Configuration version
  name: configVersion
  type: string
- description: ''
  name: owner
  type: object
- description: ''
  name: actor
  type: object
- description: Name of the resource
  name: resourceName
  type: string
- description: Identifier of the resource
  name: resourceId
  type: string
- description: URI of the resource
  name: resourceUri
  type: string
- description: Action method performed
  name: method
  type: string
- description: Activity details
  name: activity
  type: object
- description: Processed activity details
  name: processedActivity
  type: object
- description: Related sibling activities
  name: siblingActivities
  type: array
- description: Parent activity if applicable
  name: parentActivity
  type: object
- description: Parent sibling activities
  name: parentSiblingActivities
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-compliance-events-compliance-event-schema.json
slug: linkedin-compliance-events-compliance-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-compliance-events-compliance-event-schema.json\",\n  \"title\": \"ComplianceEvent\",\n  \"description\": \"ComplianceEvent from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the compliance event\",\n      \"example\": \"evt_123456789\"\n    },\n    \"capturedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Timestamp when the event was captured\",\n      \"example\": 1640000000000\n    },\n    \"processedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Timestamp when the event was processed\",\n      \"example\": 1640000001000\n    },\n    \"configVersion\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Configuration version\",\n      \"example\": \"1.0\"\n    },\n    \"owner\": {\n      \"$ref\": \"#/components/schemas/MemberProfile\"\n    },\n    \"actor\": {\n      \"$ref\": \"#/components/schemas/MemberProfile\"\n    },\n    \"resourceName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the resource\",\n      \"example\": \"MESSAGE\"\n    },\n    \"resourceId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the resource\",\n      \"example\": \"res_987654321\"\n    },\n    \"resourceUri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the resource\",\n      \"example\": \"urn:li:message:987654321\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATE\",\n        \"UPDATE\",\n        \"DELETE\"\n      ],\n      \"description\": \"Action method performed\",\n      \"example\": \"CREATE\"\n    },\n    \"activity\": {\n      \"type\": \"object\",\n      \"description\": \"Activity\
  \ details\",\n      \"additionalProperties\": true\n    },\n    \"processedActivity\": {\n      \"type\": \"object\",\n      \"description\": \"Processed activity details\",\n      \"additionalProperties\": true\n    },\n    \"siblingActivities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Related sibling activities\"\n    },\n    \"parentActivity\": {\n      \"type\": \"object\",\n      \"description\": \"Parent activity if applicable\",\n      \"additionalProperties\": true\n    },\n    \"parentSiblingActivities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Parent sibling activities\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"capturedAt\",\n    \"resourceName\",\n    \"method\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-compliance-events-compliance-event-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ComplianceEvent
---
