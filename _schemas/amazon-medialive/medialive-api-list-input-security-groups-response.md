---
description: Placeholder documentation for ListInputSecurityGroupsResponse
layout: schema
name: ListInputSecurityGroupsResponse
properties_list:
- description: ''
  name: InputSecurityGroups
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-list-input-security-groups-response-schema.json
slug: medialive-api-list-input-security-groups-response
source_filename: medialive-api-list-input-security-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-input-security-groups-response-schema.json\",\n  \"title\": \"ListInputSecurityGroupsResponse\",\n  \"description\": \"Placeholder documentation for ListInputSecurityGroupsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputSecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputSecurityGroup\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputSecurityGroups\"\n          },\n          \"description\": \"List of input security groups\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          }\n        }\n      ]\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-input-security-groups-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListInputSecurityGroupsResponse
---
