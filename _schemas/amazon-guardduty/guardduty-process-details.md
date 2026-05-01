---
description: Information about the observed process.
layout: schema
name: ProcessDetails
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: ExecutablePath
  type: object
- description: ''
  name: ExecutableSha256
  type: object
- description: ''
  name: NamespacePid
  type: object
- description: ''
  name: Pwd
  type: object
- description: ''
  name: Pid
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: Uuid
  type: object
- description: ''
  name: ParentUuid
  type: object
- description: ''
  name: User
  type: object
- description: ''
  name: UserId
  type: object
- description: ''
  name: Euid
  type: object
- description: ''
  name: Lineage
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-process-details-schema.json
slug: guardduty-process-details
source_filename: guardduty-process-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-process-details-schema.json\",\n  \"title\": \"ProcessDetails\",\n  \"description\": \"Information about the observed process.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the process.\"\n        }\n      ]\n    },\n    \"ExecutablePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"executablePath\"\n          },\n          \"description\": \"The absolute path of the process executable file.\"\n        }\n      ]\n    },\n    \"ExecutableSha256\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"executableSha256\"\n          },\n          \"description\": \"The <code>SHA256</code> hash of the process executable.\"\n        }\n      ]\n    },\n    \"NamespacePid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"namespacePid\"\n          },\n          \"description\": \"The ID of the child process.\"\n        }\n      ]\n    },\n    \"Pwd\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pwd\"\n          },\n          \"description\": \"The present working directory of the process.\"\n        }\n      ]\n    },\n    \"Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"pid\"\n          },\n          \"description\": \"The ID of the process.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"startTime\"\n          },\n          \"description\": \"The time when the process started. This is in UTC format.\"\n        }\n      ]\n    },\n    \"Uuid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"uuid\"\n          },\n          \"description\": \"The unique ID assigned to the process by GuardDuty.\"\n        }\n      ]\n    },\n    \"ParentUuid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parentUuid\"\n       \
  \   },\n          \"description\": \"The unique ID of the parent process. This ID is assigned to the parent process by GuardDuty.\"\n        }\n      ]\n    },\n    \"User\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"user\"\n          },\n          \"description\": \"The user that executed the process.\"\n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"userId\"\n          },\n          \"description\": \"The unique ID of the user that executed the process.\"\n        }\n      ]\n    },\n    \"Euid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"euid\"\n          },\n          \"description\": \"The effective user\
  \ ID of the user that executed the process.\"\n        }\n      ]\n    },\n    \"Lineage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Lineage\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lineage\"\n          },\n          \"description\": \"Information about the process's lineage.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-process-details-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ProcessDetails
---
