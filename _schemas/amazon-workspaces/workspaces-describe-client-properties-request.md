---
description: DescribeClientPropertiesRequest schema from Amazon WorkSpaces API
layout: schema
name: DescribeClientPropertiesRequest
properties_list:
- description: ''
  name: ResourceIds
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-client-properties-request-schema.json
slug: workspaces-describe-client-properties-request
source_filename: workspaces-describe-client-properties-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceIds\"\n  ],\n  \"title\": \"DescribeClientPropertiesRequest\",\n  \"properties\": {\n    \"ResourceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdList\"\n        },\n        {\n          \"description\": \"The resource identifier, in the form of directory IDs.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-client-properties-request-schema.json\",\n  \"description\": \"DescribeClientPropertiesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-client-properties-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeClientPropertiesRequest
---
