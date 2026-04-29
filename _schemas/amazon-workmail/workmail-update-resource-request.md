---
description: UpdateResourceRequest schema from Amazon WorkMail API
layout: schema
name: UpdateResourceRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: BookingOptions
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-update-resource-request-schema.json
slug: workmail-update-resource-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"ResourceId\"\n  ],\n  \"title\": \"UpdateResourceRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier associated with the organization for which the resource is updated.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier of the resource to be updated.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the resource to be updated.\"\n        }\n      ]\n    },\n    \"BookingOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/BookingOptions\"\n        },\n        {\n          \"description\": \"The resource's booking options to be updated.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-update-resource-request-schema.json\",\n  \"description\": \"UpdateResourceRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-update-resource-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: UpdateResourceRequest
---
