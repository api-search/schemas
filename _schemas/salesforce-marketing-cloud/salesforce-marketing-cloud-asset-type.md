---
description: Defines the type of an asset. Each type has a unique ID and name. Common types include htmlemail (208), templatebasedemail (207), htmlblock (197), codesnippetblock (220), and image (28).
layout: schema
name: AssetType
properties_list:
- description: Numeric identifier for the asset type
  name: id
  type: integer
- description: Name of the asset type
  name: name
  type: string
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-asset-type-schema.json
slug: salesforce-marketing-cloud-asset-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssetType\",\n  \"type\": \"object\",\n  \"description\": \"Defines the type of an asset. Each type has a unique ID and name. Common types include htmlemail (208), templatebasedemail (207), htmlblock (197), codesnippetblock (220), and image (28).\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric identifier for the asset type\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the asset type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-asset-type-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: AssetType
---
