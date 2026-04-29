---
description: DescribeResourceResponse schema from Amazon WorkMail API
layout: schema
name: DescribeResourceResponse
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: Email
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: BookingOptions
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: EnabledDate
  type: object
- description: ''
  name: DisabledDate
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-describe-resource-response-schema.json
slug: workmail-describe-resource-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier of the described resource.\"\n        }\n      ]\n    },\n    \"Email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailAddress\"\n        },\n        {\n          \"description\": \"The email of the described resource.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the described resource.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"The type of the described resource.\"\n        }\n      ]\n    },\n    \"BookingOptions\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BookingOptions\"\n        },\n        {\n          \"description\": \"The booking options for the described resource.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityState\"\n        },\n        {\n          \"description\": \"The state of the resource: enabled (registered to WorkMail), disabled (deregistered or never registered to WorkMail), or deleted.\"\n        }\n      ]\n    },\n    \"EnabledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when a resource was enabled for WorkMail, in UNIX epoch time format.\"\n        }\n      ]\n    },\n    \"DisabledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date\
  \ and time when a resource was disabled from WorkMail, in UNIX epoch time format.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeResourceResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-resource-response-schema.json\",\n  \"description\": \"DescribeResourceResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-resource-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DescribeResourceResponse
---
