---
description: Contains information about the task in an ECS cluster.
layout: schema
name: EcsTaskDetails
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: DefinitionArn
  type: object
- description: ''
  name: Version
  type: object
- description: ''
  name: TaskCreatedAt
  type: object
- description: ''
  name: StartedAt
  type: object
- description: ''
  name: StartedBy
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Volumes
  type: object
- description: ''
  name: Containers
  type: object
- description: ''
  name: Group
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-ecs-task-details-schema.json
slug: guardduty-ecs-task-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-ecs-task-details-schema.json\",\n  \"title\": \"EcsTaskDetails\",\n  \"description\": \"Contains information about the task in an ECS cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the task.\"\n        }\n      ]\n    },\n    \"DefinitionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"definitionArn\"\n          },\n          \"description\": \"The ARN of the task definition that creates the task.\"\n        }\n      ]\n\
  \    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"version\"\n          },\n          \"description\": \"The version counter for the task.\"\n        }\n      ]\n    },\n    \"TaskCreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"createdAt\"\n          },\n          \"description\": \"The Unix timestamp for the time when the task was created.\"\n        }\n      ]\n    },\n    \"StartedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"startedAt\"\n          },\n          \"description\": \"The Unix timestamp for the time when the task started.\"\n        }\n      ]\n    },\n    \"StartedBy\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"startedBy\"\n          },\n          \"description\": \"Contains the tag specified when a task is started.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags of the ECS Task.\"\n        }\n      ]\n    },\n    \"Volumes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Volumes\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"volumes\"\n          },\n          \"description\": \"The list of data volume definitions for the task.\"\n        }\n      ]\n    },\n    \"Containers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Containers\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"containers\"\n          },\n          \"description\": \"The containers that's associated with the task.\"\n        }\n      ]\n    },\n    \"Group\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"group\"\n          },\n          \"description\": \"The name of the task group that's associated with the task.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-ecs-task-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: EcsTaskDetails
---
