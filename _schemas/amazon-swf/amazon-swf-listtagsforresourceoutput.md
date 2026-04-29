---
description: ''
layout: schema
name: ListTagsForResourceOutput
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-listtagsforresourceoutput-schema.json
slug: amazon-swf-listtagsforresourceoutput
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTagList\"\n        },\n        {\n          \"description\": \"An array of tags associated with the domain.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ListTagsForResourceOutput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-listtagsforresourceoutput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ListTagsForResourceOutput
---
