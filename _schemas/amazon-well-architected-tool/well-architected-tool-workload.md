---
description: A workload return object.
layout: schema
name: Workload
properties_list:
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: WorkloadArn
  type: object
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
  name: UpdatedAt
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
  name: ArchitecturalDesign
  type: object
- description: ''
  name: ReviewOwner
  type: object
- description: ''
  name: ReviewRestrictionDate
  type: object
- description: ''
  name: IsReviewOwnerUpdateAcknowledged
  type: object
- description: ''
  name: IndustryType
  type: object
- description: ''
  name: Industry
  type: object
- description: ''
  name: Notes
  type: object
- description: ''
  name: ImprovementStatus
  type: object
- description: ''
  name: RiskCounts
  type: object
- description: ''
  name: PillarPriorities
  type: object
- description: ''
  name: Lenses
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: ShareInvitationId
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
  name: Profiles
  type: object
- description: ''
  name: PrioritizedRiskCounts
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-workload-schema.json
slug: well-architected-tool-workload
source_filename: well-architected-tool-workload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"WorkloadArn\": {\n      \"$ref\": \"#/components/schemas/WorkloadArn\"\n    },\n    \"WorkloadName\": {\n      \"$ref\": \"#/components/schemas/WorkloadName\"\n    },\n    \"Description\": {\n      \"$ref\": \"#/components/schemas/WorkloadDescription\"\n    },\n    \"Environment\": {\n      \"$ref\": \"#/components/schemas/WorkloadEnvironment\"\n    },\n    \"UpdatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"AccountIds\": {\n      \"$ref\": \"#/components/schemas/WorkloadAccountIds\"\n    },\n    \"AwsRegions\": {\n      \"$ref\": \"#/components/schemas/WorkloadAwsRegions\"\n    },\n    \"NonAwsRegions\": {\n      \"$ref\": \"#/components/schemas/WorkloadNonAwsRegions\"\n    },\n    \"ArchitecturalDesign\": {\n      \"$ref\": \"#/components/schemas/WorkloadArchitecturalDesign\"\n    },\n    \"ReviewOwner\"\
  : {\n      \"$ref\": \"#/components/schemas/WorkloadReviewOwner\"\n    },\n    \"ReviewRestrictionDate\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"IsReviewOwnerUpdateAcknowledged\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IsReviewOwnerUpdateAcknowledged\"\n        },\n        {\n          \"description\": \"<p>Flag indicating whether the workload owner has acknowledged that the <i>Review owner</i> field is required.</p> <p>If a <b>Review owner</b> is not added to the workload within 60 days of acknowledgement, access to the workload is restricted until an owner is added.</p>\"\n        }\n      ]\n    },\n    \"IndustryType\": {\n      \"$ref\": \"#/components/schemas/WorkloadIndustryType\"\n    },\n    \"Industry\": {\n      \"$ref\": \"#/components/schemas/WorkloadIndustry\"\n    },\n    \"Notes\": {\n      \"$ref\": \"#/components/schemas/Notes\"\n    },\n    \"ImprovementStatus\": {\n      \"$ref\": \"#/components/schemas/WorkloadImprovementStatus\"\
  \n    },\n    \"RiskCounts\": {\n      \"$ref\": \"#/components/schemas/RiskCounts\"\n    },\n    \"PillarPriorities\": {\n      \"$ref\": \"#/components/schemas/WorkloadPillarPriorities\"\n    },\n    \"Lenses\": {\n      \"$ref\": \"#/components/schemas/WorkloadLenses\"\n    },\n    \"Owner\": {\n      \"$ref\": \"#/components/schemas/AwsAccountId\"\n    },\n    \"ShareInvitationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareInvitationId\"\n        },\n        {\n          \"description\": \"The ID assigned to the share invitation.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags associated with the workload.\"\n        }\n      ]\n    },\n    \"DiscoveryConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkloadDiscoveryConfig\"\n        },\n        {\n          \"\
  description\": \"Discovery configuration associated to the workload.\"\n        }\n      ]\n    },\n    \"Applications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkloadApplications\"\n        },\n        {\n          \"description\": \"List of AppRegistry application ARNs associated to the workload.\"\n        }\n      ]\n    },\n    \"Profiles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkloadProfiles\"\n        },\n        {\n          \"description\": \"Profile associated with a workload.\"\n        }\n      ]\n    },\n    \"PrioritizedRiskCounts\": {\n      \"$ref\": \"#/components/schemas/RiskCounts\"\n    }\n  },\n  \"description\": \"A workload return object.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Workload\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: Workload
---
