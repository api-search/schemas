---
description: DisassociateDelegateFromResourceRequest schema from Amazon WorkMail API
layout: schema
name: DisassociateDelegateFromResourceRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: EntityId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-disassociate-delegate-from-resource-request-schema.json
slug: workmail-disassociate-delegate-from-resource-request
source_filename: workmail-disassociate-delegate-from-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"ResourceId\",\n    \"EntityId\"\n  ],\n  \"title\": \"DisassociateDelegateFromResourceRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier for the organization under which the resource exists.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier of the resource from which delegates' set members are removed. \"\n        }\n      ]\n    },\n    \"EntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier for the member (user, group) to be removed from the resource's\
  \ delegates.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-disassociate-delegate-from-resource-request-schema.json\",\n  \"description\": \"DisassociateDelegateFromResourceRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-disassociate-delegate-from-resource-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DisassociateDelegateFromResourceRequest
---
