---
description: AssociateIpGroupsRequest schema from Amazon WorkSpaces API
layout: schema
name: AssociateIpGroupsRequest
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: GroupIds
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-associate-ip-groups-request-schema.json
slug: workspaces-associate-ip-groups-request
source_filename: workspaces-associate-ip-groups-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"DirectoryId\",\n    \"GroupIds\"\n  ],\n  \"title\": \"AssociateIpGroupsRequest\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the directory.\"\n        }\n      ]\n    },\n    \"GroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupIdList\"\n        },\n        {\n          \"description\": \"The identifiers of one or more IP access control groups.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-associate-ip-groups-request-schema.json\",\n  \"description\": \"AssociateIpGroupsRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-associate-ip-groups-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: AssociateIpGroupsRequest
---
