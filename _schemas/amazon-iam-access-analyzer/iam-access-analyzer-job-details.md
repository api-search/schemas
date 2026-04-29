---
description: Contains details about the policy generation request.
layout: schema
name: JobDetails
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: startedOn
  type: object
- description: ''
  name: completedOn
  type: object
- description: ''
  name: jobError
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-job-details-schema.json
slug: iam-access-analyzer-job-details
source_filename: iam-access-analyzer-job-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-job-details-schema.json\",\n  \"title\": \"JobDetails\",\n  \"description\": \"Contains details about the policy generation request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The <code>JobId</code> that is returned by the <code>StartPolicyGeneration</code> operation. The <code>JobId</code> can be used with <code>GetGeneratedPolicy</code> to retrieve the generated policies or used with <code>CancelPolicyGeneration</code> to cancel the policy generation request.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n      \
  \  {\n          \"description\": \"The status of the job request.\"\n        }\n      ]\n    },\n    \"startedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp of when the job was started.\"\n        }\n      ]\n    },\n    \"completedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp of when the job was completed.\"\n        }\n      ]\n    },\n    \"jobError\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobError\"\n        },\n        {\n          \"description\": \"The job error for the policy generation request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobId\",\n    \"status\",\n    \"startedOn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-job-details-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: JobDetails
---
