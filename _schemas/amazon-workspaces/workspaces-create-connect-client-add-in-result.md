---
description: CreateConnectClientAddInResult schema from Amazon WorkSpaces API
layout: schema
name: CreateConnectClientAddInResult
properties_list:
- description: ''
  name: AddInId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-connect-client-add-in-result-schema.json
slug: workspaces-create-connect-client-add-in-result
source_filename: workspaces-create-connect-client-add-in-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AddInId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonUuid\"\n        },\n        {\n          \"description\": \"The client add-in identifier.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateConnectClientAddInResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-connect-client-add-in-result-schema.json\",\n  \"description\": \"CreateConnectClientAddInResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-connect-client-add-in-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateConnectClientAddInResult
---
