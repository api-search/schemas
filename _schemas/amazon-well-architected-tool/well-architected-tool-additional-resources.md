---
description: <p>The choice level additional resources for a custom lens.</p> <p>This field does not apply to Amazon Web Services official lenses.</p>
layout: schema
name: AdditionalResources
properties_list:
- description: ''
  name: Type
  type: object
- description: ''
  name: Content
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-additional-resources-schema.json
slug: well-architected-tool-additional-resources
source_filename: well-architected-tool-additional-resources-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdditionalResourceType\"\n        },\n        {\n          \"description\": \"Type of additional resource for a custom lens.\"\n        }\n      ]\n    },\n    \"Content\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Urls\"\n        },\n        {\n          \"description\": \"The URLs for additional resources, either helpful resources or improvement plans, for a custom lens. Up to five additional URLs can be specified.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p>The choice level additional resources for a custom lens.</p> <p>This field does not apply to Amazon Web Services official lenses.</p>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AdditionalResources\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-additional-resources-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-additional-resources-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: AdditionalResources
---
