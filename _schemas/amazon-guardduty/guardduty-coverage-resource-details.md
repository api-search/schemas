---
description: Information about the resource for each individual EKS cluster.
layout: schema
name: CoverageResourceDetails
properties_list:
- description: ''
  name: EksClusterDetails
  type: object
- description: ''
  name: ResourceType
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-coverage-resource-details-schema.json
slug: guardduty-coverage-resource-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-resource-details-schema.json\",\n  \"title\": \"CoverageResourceDetails\",\n  \"description\": \"Information about the resource for each individual EKS cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EksClusterDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageEksClusterDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"eksClusterDetails\"\n          },\n          \"description\": \"EKS cluster details involved in the coverage statistics.\"\n        }\n      ]\n    },\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceType\"\n          },\n          \"description\"\
  : \"The type of Amazon Web Services resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-resource-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CoverageResourceDetails
---
