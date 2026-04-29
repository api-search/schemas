---
description: Input for workload creation.
layout: schema
name: CreateWorkloadInput
properties_list:
- description: ''
  name: WorkloadName
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Environment
  type: object
- description: ''
  name: AccountIds
  type: object
- description: ''
  name: AwsRegions
  type: object
- description: ''
  name: NonAwsRegions
  type: object
- description: ''
  name: PillarPriorities
  type: object
- description: ''
  name: ArchitecturalDesign
  type: object
- description: ''
  name: ReviewOwner
  type: object
- description: ''
  name: IndustryType
  type: object
- description: ''
  name: Industry
  type: object
- description: ''
  name: Lenses
  type: object
- description: ''
  name: Notes
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: DiscoveryConfig
  type: object
- description: ''
  name: Applications
  type: object
- description: ''
  name: ProfileArns
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-create-workload-input-schema.json
slug: well-architected-tool-create-workload-input
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"WorkloadName\",\n    \"Description\",\n    \"Environment\",\n    \"Lenses\",\n    \"ClientRequestToken\"\n  ],\n  \"title\": \"CreateWorkloadInput\",\n  \"properties\": {\n    \"WorkloadName\": {\n      \"$ref\": \"#/components/schemas/WorkloadName\"\n    },\n    \"Description\": {\n      \"$ref\": \"#/components/schemas/WorkloadDescription\"\n    },\n    \"Environment\": {\n      \"$ref\": \"#/components/schemas/WorkloadEnvironment\"\n    },\n    \"AccountIds\": {\n      \"$ref\": \"#/components/schemas/WorkloadAccountIds\"\n    },\n    \"AwsRegions\": {\n      \"$ref\": \"#/components/schemas/WorkloadAwsRegions\"\n    },\n    \"NonAwsRegions\": {\n      \"$ref\": \"#/components/schemas/WorkloadNonAwsRegions\"\n    },\n    \"PillarPriorities\": {\n      \"$ref\": \"#/components/schemas/WorkloadPillarPriorities\"\n    },\n    \"ArchitecturalDesign\": {\n      \"$ref\": \"#/components/schemas/WorkloadArchitecturalDesign\"\n\
  \    },\n    \"ReviewOwner\": {\n      \"$ref\": \"#/components/schemas/WorkloadReviewOwner\"\n    },\n    \"IndustryType\": {\n      \"$ref\": \"#/components/schemas/WorkloadIndustryType\"\n    },\n    \"Industry\": {\n      \"$ref\": \"#/components/schemas/WorkloadIndustry\"\n    },\n    \"Lenses\": {\n      \"$ref\": \"#/components/schemas/WorkloadLenses\"\n    },\n    \"Notes\": {\n      \"$ref\": \"#/components/schemas/Notes\"\n    },\n    \"ClientRequestToken\": {\n      \"$ref\": \"#/components/schemas/ClientRequestToken\"\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags to be associated with the workload.\"\n        }\n      ]\n    },\n    \"DiscoveryConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkloadDiscoveryConfig\"\n        },\n        {\n          \"description\": \"Well-Architected discovery configuration settings\
  \ associated to the workload.\"\n        }\n      ]\n    },\n    \"Applications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkloadApplications\"\n        },\n        {\n          \"description\": \"List of AppRegistry application ARNs associated to the workload.\"\n        }\n      ]\n    },\n    \"ProfileArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkloadProfileArns\"\n        },\n        {\n          \"description\": \"The list of profile ARNs associated with the workload.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Input for workload creation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-workload-input-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-workload-input-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: CreateWorkloadInput
---
