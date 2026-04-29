---
description: Details about the Systems Manager automation document that will be used as a runbook during an incident.
layout: schema
name: SsmAutomation
properties_list:
- description: ''
  name: documentName
  type: object
- description: ''
  name: documentVersion
  type: object
- description: ''
  name: dynamicParameters
  type: object
- description: ''
  name: parameters
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: targetAccount
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-ssm-automation-schema.json
slug: incident-manager-ssm-automation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-ssm-automation-schema.json\",\n  \"title\": \"SsmAutomation\",\n  \"description\": \"Details about the Systems Manager automation document that will be used as a runbook during an incident.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"documentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SsmAutomationDocumentNameString\"\n        },\n        {\n          \"description\": \"The automation document's name.\"\n        }\n      ]\n    },\n    \"documentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SsmAutomationDocumentVersionString\"\n        },\n        {\n          \"description\": \"The automation document's version to use when running.\"\n        }\n      ]\n    },\n    \"dynamicParameters\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DynamicSsmParameters\"\n        },\n        {\n          \"description\": \"The key-value pair to resolve dynamic parameter values when processing a Systems Manager Automation runbook.\"\n        }\n      ]\n    },\n    \"parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SsmParameters\"\n        },\n        {\n          \"description\": \"The key-value pair parameters to use when running the automation document.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the role that the automation document will assume when running commands.\"\n        }\n      ]\n    },\n    \"targetAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SsmTargetAccount\"\n        },\n     \
  \   {\n          \"description\": \"The account that the automation document will be run in. This can be in either the management account or an application account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"documentName\",\n    \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-ssm-automation-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: SsmAutomation
---
