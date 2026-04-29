---
description: ListPortalsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: ListPortalsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: portals
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-list-portals-response-schema.json
slug: workspaces-web-list-portals-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The pagination token used to retrieve the next page of results for this operation. \"\n        }\n      ]\n    },\n    \"portals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortalList\"\n        },\n        {\n          \"description\": \"The portals in the list.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListPortalsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-list-portals-response-schema.json\",\n  \"description\": \"ListPortalsResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-list-portals-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: ListPortalsResponse
---
