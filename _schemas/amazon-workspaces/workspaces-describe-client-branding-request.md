---
description: DescribeClientBrandingRequest schema from Amazon WorkSpaces API
layout: schema
name: DescribeClientBrandingRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-client-branding-request-schema.json
slug: workspaces-describe-client-branding-request
source_filename: workspaces-describe-client-branding-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceId\"\n  ],\n  \"title\": \"DescribeClientBrandingRequest\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The directory identifier of the WorkSpace for which you want to view client branding information.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-client-branding-request-schema.json\",\n  \"description\": \"DescribeClientBrandingRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-client-branding-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeClientBrandingRequest
---
