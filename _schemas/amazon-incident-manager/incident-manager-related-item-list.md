---
description: RelatedItemList schema
layout: schema
name: RelatedItemList
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-related-item-list-schema.json
slug: incident-manager-related-item-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-related-item-list-schema.json\",\n  \"title\": \"RelatedItemList\",\n  \"description\": \"RelatedItemList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"identifier\"\n    ],\n    \"properties\": {\n      \"generatedId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/GeneratedId\"\n          },\n          {\n            \"description\": \"<p>A unique ID for a <code>RelatedItem</code>.</p> <important> <p>Don't specify this parameter when you add a <code>RelatedItem</code> by using the <a>UpdateRelatedItems</a> API action.</p> </important>\"\n          }\n        ]\n      },\n      \"identifier\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ItemIdentifier\"\
  \n          },\n          {\n            \"description\": \"Details about the related item.\"\n          }\n        ]\n      },\n      \"title\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/RelatedItemTitleString\"\n          },\n          {\n            \"description\": \"The title of the related item.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Resources that responders use to triage and mitigate the incident.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-related-item-list-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: RelatedItemList
---
