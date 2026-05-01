---
description: Details of a container.
layout: schema
name: Container
properties_list:
- description: ''
  name: ContainerRuntime
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Image
  type: object
- description: ''
  name: ImagePrefix
  type: object
- description: ''
  name: VolumeMounts
  type: object
- description: ''
  name: SecurityContext
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-container-schema.json
slug: guardduty-container
source_filename: guardduty-container-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-container-schema.json\",\n  \"title\": \"Container\",\n  \"description\": \"Details of a container.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContainerRuntime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"containerRuntime\"\n          },\n          \"description\": \"The container runtime (such as, Docker or containerd) used to run the container.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"Container ID.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Container name.\"\n        }\n      ]\n    },\n    \"Image\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"image\"\n          },\n          \"description\": \"Container image.\"\n        }\n      ]\n    },\n    \"ImagePrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imagePrefix\"\n          },\n          \"description\": \"Part of the image name before the last slash. For example, imagePrefix for public.ecr.aws/amazonlinux/amazonlinux:latest would be public.ecr.aws/amazonlinux. If the image name is relative and does not have a slash, this field is empty.\"\n        }\n      ]\n\
  \    },\n    \"VolumeMounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeMounts\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"volumeMounts\"\n          },\n          \"description\": \"Container volume mounts.\"\n        }\n      ]\n    },\n    \"SecurityContext\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityContext\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityContext\"\n          },\n          \"description\": \"Container security context.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-container-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Container
---
