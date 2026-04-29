---
description: Contains information about the details of the ECS Cluster.
layout: schema
name: EcsClusterDetails
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: ActiveServicesCount
  type: object
- description: ''
  name: RegisteredContainerInstancesCount
  type: object
- description: ''
  name: RunningTasksCount
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: TaskDetails
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-ecs-cluster-details-schema.json
slug: guardduty-ecs-cluster-details
source_filename: guardduty-ecs-cluster-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-ecs-cluster-details-schema.json\",\n  \"title\": \"EcsClusterDetails\",\n  \"description\": \"Contains information about the details of the ECS Cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the ECS Cluster.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the cluster.\"\n        }\n      ]\n    },\n    \"Status\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"The status of the ECS cluster.\"\n        }\n      ]\n    },\n    \"ActiveServicesCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"activeServicesCount\"\n          },\n          \"description\": \"The number of services that are running on the cluster in an ACTIVE state.\"\n        }\n      ]\n    },\n    \"RegisteredContainerInstancesCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"registeredContainerInstancesCount\"\n          },\n          \"description\": \"The number of container instances registered into the cluster.\"\n        }\n      ]\n  \
  \  },\n    \"RunningTasksCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"runningTasksCount\"\n          },\n          \"description\": \"The number of tasks in the cluster that are in the RUNNING state.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags of the ECS Cluster.\"\n        }\n      ]\n    },\n    \"TaskDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcsTaskDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"taskDetails\"\n          },\n          \"description\": \"Contains information about the details of the ECS Task.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-ecs-cluster-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: EcsClusterDetails
---
