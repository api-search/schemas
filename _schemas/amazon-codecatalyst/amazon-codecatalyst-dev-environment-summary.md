---
description: Information about a Dev Environment.
layout: schema
name: DevEnvironmentSummary
properties_list:
- description: ''
  name: spaceName
  type: object
- description: ''
  name: projectName
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: lastUpdatedTime
  type: object
- description: ''
  name: creatorId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusReason
  type: object
- description: ''
  name: repositories
  type: object
- description: ''
  name: alias
  type: object
- description: ''
  name: ides
  type: object
- description: ''
  name: instanceType
  type: object
- description: ''
  name: inactivityTimeoutMinutes
  type: object
- description: ''
  name: persistentStorage
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-dev-environment-summary-schema.json
slug: amazon-codecatalyst-dev-environment-summary
source_filename: amazon-codecatalyst-dev-environment-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-dev-environment-summary-schema.json\",\n  \"title\": \"DevEnvironmentSummary\",\n  \"description\": \"Information about a Dev Environment. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the space.\"\n        }\n      ]\n    },\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the project in the space.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"\
  The system-generated unique ID for the Dev Environment. \"\n        }\n      ]\n    },\n    \"lastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The time when the Dev Environment was last updated, in coordinated universal time (UTC) timestamp format as specified in <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\\\">RFC 3339</a>.\"\n        }\n      ]\n    },\n    \"creatorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEnvironmentSummaryCreatorIdString\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the user who created the Dev Environment. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEnvironmentStatus\"\n        },\n        {\n          \"description\": \"The status of the Dev Environment.\
  \ \"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusReason\"\n        },\n        {\n          \"description\": \"The reason for the status.\"\n        }\n      ]\n    },\n    \"repositories\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEnvironmentRepositorySummaries\"\n        },\n        {\n          \"description\": \"Information about the repositories that will be cloned into the Dev Environment. If no rvalue is specified, no repository is cloned.\"\n        }\n      ]\n    },\n    \"alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEnvironmentSummaryAliasString\"\n        },\n        {\n          \"description\": \"The user-specified alias for the Dev Environment.\"\n        }\n      ]\n    },\n    \"ides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ides\"\n        },\n        {\n     \
  \     \"description\": \"Information about the integrated development environment (IDE) configured for a Dev Environment.\"\n        }\n      ]\n    },\n    \"instanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceType\"\n        },\n        {\n          \"description\": \"The Amazon EC2 instace type used for the Dev Environment. \"\n        }\n      ]\n    },\n    \"inactivityTimeoutMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InactivityTimeoutMinutes\"\n        },\n        {\n          \"description\": \"The amount of time the Dev Environment will run without any activity detected before stopping, in minutes. Dev Environments consume compute minutes when running.\"\n        }\n      ]\n    },\n    \"persistentStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PersistentStorage\"\n        },\n        {\n          \"description\": \"Information about the configuration\
  \ of persistent storage for the Dev Environment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"lastUpdatedTime\",\n    \"creatorId\",\n    \"status\",\n    \"repositories\",\n    \"instanceType\",\n    \"inactivityTimeoutMinutes\",\n    \"persistentStorage\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-dev-environment-summary-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: DevEnvironmentSummary
---
