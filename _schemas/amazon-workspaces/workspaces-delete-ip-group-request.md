---
description: DeleteIpGroupRequest schema from Amazon WorkSpaces API
layout: schema
name: DeleteIpGroupRequest
properties_list:
- description: ''
  name: GroupId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-delete-ip-group-request-schema.json
slug: workspaces-delete-ip-group-request
source_filename: workspaces-delete-ip-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"GroupId\"\n  ],\n  \"title\": \"DeleteIpGroupRequest\",\n  \"properties\": {\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupId\"\n        },\n        {\n          \"description\": \"The identifier of the IP access control group.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-delete-ip-group-request-schema.json\",\n  \"description\": \"DeleteIpGroupRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-delete-ip-group-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DeleteIpGroupRequest
---
