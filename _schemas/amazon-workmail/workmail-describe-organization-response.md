---
description: DescribeOrganizationResponse schema from Amazon WorkMail API
layout: schema
name: DescribeOrganizationResponse
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: Alias
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: DirectoryType
  type: object
- description: ''
  name: DefaultMailDomain
  type: object
- description: ''
  name: CompletedDate
  type: object
- description: ''
  name: ErrorMessage
  type: object
- description: ''
  name: ARN
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-describe-organization-response-schema.json
slug: workmail-describe-organization-response
source_filename: workmail-describe-organization-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier of an organization.\"\n        }\n      ]\n    },\n    \"Alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationName\"\n        },\n        {\n          \"description\": \"The alias for an organization.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The state of an organization.\"\n        }\n      ]\n    },\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier for the directory associated with an WorkMail organization.\"\n        }\n      ]\n  \
  \  },\n    \"DirectoryType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of directory associated with the WorkMail organization.\"\n        }\n      ]\n    },\n    \"DefaultMailDomain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The default mail domain associated with the organization.\"\n        }\n      ]\n    },\n    \"CompletedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date at which the organization became usable in the WorkMail context, in UNIX epoch time format.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"(Optional) The error message\
  \ indicating if unexpected behavior was encountered with regards to the organization.\"\n        }\n      ]\n    },\n    \"ARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the organization.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeOrganizationResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-organization-response-schema.json\",\n  \"description\": \"DescribeOrganizationResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-organization-response-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DescribeOrganizationResponse
---
