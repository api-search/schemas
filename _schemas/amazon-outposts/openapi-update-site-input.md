---
description: UpdateSiteInput schema from Amazon Outposts
layout: schema
name: UpdateSiteInput
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Notes
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-update-site-input-schema.json
slug: openapi-update-site-input
source_filename: openapi-update-site-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-update-site-input-schema.json\",\n  \"title\": \"UpdateSiteInput\",\n  \"description\": \"UpdateSiteInput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"$ref\": \"#/components/schemas/SiteName\"\n    },\n    \"Description\": {\n      \"$ref\": \"#/components/schemas/SiteDescription\"\n    },\n    \"Notes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SiteNotes\"\n        },\n        {\n          \"description\": \"Notes about a site.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-update-site-input-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: UpdateSiteInput
---
