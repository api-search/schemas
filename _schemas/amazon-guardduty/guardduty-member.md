---
description: Contains information about the member account.
layout: schema
name: Member
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: DetectorId
  type: object
- description: ''
  name: MasterId
  type: object
- description: ''
  name: Email
  type: object
- description: ''
  name: RelationshipStatus
  type: object
- description: ''
  name: InvitedAt
  type: object
- description: ''
  name: UpdatedAt
  type: object
- description: ''
  name: AdministratorId
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-member-schema.json
slug: guardduty-member
source_filename: guardduty-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-member-schema.json\",\n  \"title\": \"Member\",\n  \"description\": \"Contains information about the member account. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountId\"\n          },\n          \"description\": \"The ID of the member account.\"\n        }\n      ]\n    },\n    \"DetectorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"detectorId\"\n          },\n          \"description\": \"The detector ID of the member account.\"\n        }\n      ]\n    },\n    \"MasterId\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"masterId\"\n          },\n          \"description\": \"The administrator account ID.\"\n        }\n      ]\n    },\n    \"Email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Email\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"email\"\n          },\n          \"description\": \"The email address of the member account.\"\n        }\n      ]\n    },\n    \"RelationshipStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"relationshipStatus\"\n          },\n          \"description\": \"The status of the relationship between the member and the administrator.\"\n        }\n      ]\n    },\n    \"InvitedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"invitedAt\"\n          },\n          \"description\": \"The timestamp when the invitation was sent.\"\n        }\n      ]\n    },\n    \"UpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"updatedAt\"\n          },\n          \"description\": \"The last-updated timestamp of the member.\"\n        }\n      ]\n    },\n    \"AdministratorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"administratorId\"\n          },\n          \"description\": \"The administrator account ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountId\",\n    \"MasterId\",\n    \"Email\",\n    \"RelationshipStatus\",\n    \"UpdatedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-member-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Member
---
