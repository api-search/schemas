---
description: DescribeGroupResponse schema from Amazon WorkMail API
layout: schema
name: DescribeGroupResponse
properties_list:
- description: ''
  name: GroupId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Email
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
schema_file: json-schema/workmail-describe-group-response-schema.json
slug: workmail-describe-group-response
source_filename: workmail-describe-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the described group.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupName\"\n        },\n        {\n          \"description\": \"The name of the described group.\"\n        }\n      ]\n    },\n    \"Email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailAddress\"\n        },\n        {\n          \"description\": \"The email of the described group.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityState\"\n        },\n        {\n          \"description\": \"The state of the user: enabled (registered to WorkMail) or disabled (deregistered or never registered\
  \ to WorkMail).\"\n        }\n      ]\n    },\n    \"EnabledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when a user was registered to WorkMail, in UNIX epoch time format.\"\n        }\n      ]\n    },\n    \"DisabledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when a user was deregistered from WorkMail, in UNIX epoch time format.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeGroupResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-group-response-schema.json\",\n  \"description\": \"DescribeGroupResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-group-response-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DescribeGroupResponse
---
