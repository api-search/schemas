---
description: At least one delegate must be associated to the resource to disable automatic replies from the resource.
layout: schema
name: BookingOptions
properties_list:
- description: ''
  name: AutoAcceptRequests
  type: object
- description: ''
  name: AutoDeclineRecurringRequests
  type: object
- description: ''
  name: AutoDeclineConflictingRequests
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-booking-options-schema.json
slug: workmail-booking-options
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoAcceptRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The resource's ability to automatically reply to requests. If disabled, delegates must be associated to the resource.\"\n        }\n      ]\n    },\n    \"AutoDeclineRecurringRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The resource's ability to automatically decline any recurring requests.\"\n        }\n      ]\n    },\n    \"AutoDeclineConflictingRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The resource's ability to automatically decline any conflicting requests.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"At least one delegate must be\
  \ associated to the resource to disable automatic replies from the resource.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BookingOptions\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-booking-options-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-booking-options-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: BookingOptions
---
