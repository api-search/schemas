---
description: Information about the runtime process details.
layout: schema
name: LineageObject
properties_list:
- description: ''
  name: StartTime
  type: object
- description: ''
  name: NamespacePid
  type: object
- description: ''
  name: UserId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Pid
  type: object
- description: ''
  name: Uuid
  type: object
- description: ''
  name: ExecutablePath
  type: object
- description: ''
  name: Euid
  type: object
- description: ''
  name: ParentUuid
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-lineage-object-schema.json
slug: guardduty-lineage-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-lineage-object-schema.json\",\n  \"title\": \"LineageObject\",\n  \"description\": \"Information about the runtime process details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"startTime\"\n          },\n          \"description\": \"The time when the process started. This is in UTC format.\"\n        }\n      ]\n    },\n    \"NamespacePid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"namespacePid\"\n          },\n          \"description\": \"The process ID of the child process.\"\n        }\n      ]\n\
  \    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"userId\"\n          },\n          \"description\": \"The user ID of the user that executed the process.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the process.\"\n        }\n      ]\n    },\n    \"Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pid\"\n          },\n          \"description\": \"The ID of the process.\"\n        }\n      ]\n    },\n    \"Uuid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n       \
  \   \"xml\": {\n            \"name\": \"uuid\"\n          },\n          \"description\": \"The unique ID assigned to the process by GuardDuty.\"\n        }\n      ]\n    },\n    \"ExecutablePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"executablePath\"\n          },\n          \"description\": \"The absolute path of the process executable file.\"\n        }\n      ]\n    },\n    \"Euid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"euid\"\n          },\n          \"description\": \"The effective user ID that was used to execute the process.\"\n        }\n      ]\n    },\n    \"ParentUuid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parentUuid\"\n\
  \          },\n          \"description\": \"The unique ID of the parent process. This ID is assigned to the parent process by GuardDuty.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-lineage-object-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: LineageObject
---
