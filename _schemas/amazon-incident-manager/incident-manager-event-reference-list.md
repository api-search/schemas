---
description: EventReferenceList schema
layout: schema
name: EventReferenceList
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-event-reference-list-schema.json
slug: incident-manager-event-reference-list
source_filename: incident-manager-event-reference-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-event-reference-list-schema.json\",\n  \"title\": \"EventReferenceList\",\n  \"description\": \"EventReferenceList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"relatedItemId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/GeneratedId\"\n          },\n          {\n            \"description\": \"The ID of a <code>RelatedItem</code> referenced in a <code>TimelineEvent</code>.\"\n          }\n        ]\n      },\n      \"resource\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Arn\"\n          },\n          {\n            \"description\": \"The Amazon Resource Name (ARN) of an Amazon Web Services resource referenced in a <code>TimelineEvent</code>.\"\
  \n          }\n        ]\n      }\n    },\n    \"description\": \"An item referenced in a <code>TimelineEvent</code> that is involved in or somehow associated with an incident. You can specify an Amazon Resource Name (ARN) for an Amazon Web Services resource or a <code>RelatedItem</code> ID.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-event-reference-list-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: EventReferenceList
---
