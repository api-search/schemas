---
description: GetMatchingWorkflowOutput schema from AWS EntityResolution
layout: schema
name: GetMatchingWorkflowOutput
properties_list:
- description: ''
  name: createdAt
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: incrementalRunConfig
  type: object
- description: ''
  name: inputSourceConfig
  type: object
- description: ''
  name: outputSourceConfig
  type: object
- description: ''
  name: resolutionTechniques
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: tags
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
schema_file: json-schema/amazon-entity-resolution-get-matching-workflow-output-schema.json
slug: amazon-entity-resolution-get-matching-workflow-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-get-matching-workflow-output-schema.json\",\n  \"title\": \"GetMatchingWorkflowOutput\",\n  \"description\": \"GetMatchingWorkflowOutput schema from AWS EntityResolution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp of when the workflow was created.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the workflow.\"\n        }\n      ]\n    },\n    \"incrementalRunConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncrementalRunConfig\"\
  \n        },\n        {\n          \"description\": \"An object which defines an incremental run type and has only <code>incrementalRunType</code> as a field.\"\n        }\n      ]\n    },\n    \"inputSourceConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputSourceConfig\"\n        },\n        {\n          \"description\": \"A list of <code>InputSource</code> objects, which have the fields <code>InputSourceARN</code> and <code>SchemaName</code>.\"\n        }\n      ]\n    },\n    \"outputSourceConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputSourceConfig\"\n        },\n        {\n          \"description\": \"A list of <code>OutputSource</code> objects, each of which contains fields <code>OutputS3Path</code>, <code>ApplyNormalization</code>, and <code>Output</code>.\"\n        }\n      ]\n    },\n    \"resolutionTechniques\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolutionTechniques\"\
  \n        },\n        {\n          \"description\": \"An object which defines the <code>resolutionType</code> and the <code>ruleBasedProperties</code> \"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role. AWS Entity Resolution assumes this role to access resources on your behalf.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags used to organize, track, or control access for this resource.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp of when the workflow was last updated.\"\n        }\n      ]\n    },\n    \"\
  workflowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchingWorkflowArn\"\n        },\n        {\n          \"description\": \"The ARN (Amazon Resource Name) that Entity Resolution generated for the <code>MatchingWorkflow</code>.\"\n        }\n      ]\n    },\n    \"workflowName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the workflow.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"createdAt\",\n    \"inputSourceConfig\",\n    \"outputSourceConfig\",\n    \"resolutionTechniques\",\n    \"roleArn\",\n    \"updatedAt\",\n    \"workflowArn\",\n    \"workflowName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-get-matching-workflow-output-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: GetMatchingWorkflowOutput
---
