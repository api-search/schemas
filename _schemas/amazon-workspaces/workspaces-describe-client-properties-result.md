---
description: DescribeClientPropertiesResult schema from Amazon WorkSpaces API
layout: schema
name: DescribeClientPropertiesResult
properties_list:
- description: ''
  name: ClientPropertiesList
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-client-properties-result-schema.json
slug: workspaces-describe-client-properties-result
source_filename: workspaces-describe-client-properties-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientPropertiesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientPropertiesList\"\n        },\n        {\n          \"description\": \"Information about the specified Amazon WorkSpaces clients.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeClientPropertiesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-client-properties-result-schema.json\",\n  \"description\": \"DescribeClientPropertiesResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-client-properties-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeClientPropertiesResult
---
