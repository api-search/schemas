---
description: A list of <code>MatchingWorkflowSummary</code> objects, each of which contain the fields <code>WorkflowName</code>, <code>WorkflowArn</code>, <code>CreatedAt</code>, <code>UpdatedAt</code>.
layout: schema
name: MatchingWorkflowSummary
properties_list:
- description: ''
  name: createdAt
  type: object
- description: ''
  name: updatedAt
  type: object
- description: ''
  name: workflowArn
  type: object
- description: ''
  name: workflowName
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-matching-workflow-summary-schema.json
slug: amazon-entity-resolution-matching-workflow-summary
source_filename: amazon-entity-resolution-matching-workflow-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-matching-workflow-summary-schema.json\",\n  \"title\": \"MatchingWorkflowSummary\",\n  \"description\": \"A list of <code>MatchingWorkflowSummary</code> objects, each of which contain the fields <code>WorkflowName</code>, <code>WorkflowArn</code>, <code>CreatedAt</code>, <code>UpdatedAt</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp of when the workflow was created.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp of when the workflow\
  \ was last updated.\"\n        }\n      ]\n    },\n    \"workflowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchingWorkflowArn\"\n        },\n        {\n          \"description\": \"The ARN (Amazon Resource Name) that Entity Resolution generated for the <code>MatchingWorkflow</code>.\"\n        }\n      ]\n    },\n    \"workflowName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the workflow.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"createdAt\",\n    \"updatedAt\",\n    \"workflowArn\",\n    \"workflowName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-matching-workflow-summary-schema.json
tags:
- Amazon Web Services
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: MatchingWorkflowSummary
---
