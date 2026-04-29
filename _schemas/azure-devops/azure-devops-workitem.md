---
description: JSON Schema for an Azure DevOps work item (Bug, Task, User Story, Epic, Feature, etc.).
layout: schema
name: Azure DevOps Work Item
properties_list:
- description: Work item ID
  name: id
  type: integer
- description: Work item revision number
  name: rev
  type: integer
- description: Work item field values keyed by reference name
  name: fields
  type: object
- description: Links to related work items and artifacts
  name: relations
  type: array
- description: API URL for the work item
  name: url
  type: string
provider_name: Azure DevOps
provider_slug: azure-devops
schema_file: json-schema/azure-devops-workitem-schema.json
slug: azure-devops-workitem
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-workitem-schema.json\",\n  \"title\": \"Azure DevOps Work Item\",\n  \"description\": \"JSON Schema for an Azure DevOps work item (Bug, Task, User Story, Epic, Feature, etc.).\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"rev\", \"fields\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Work item ID\",\n      \"minimum\": 1\n    },\n    \"rev\": {\n      \"type\": \"integer\",\n      \"description\": \"Work item revision number\",\n      \"minimum\": 1\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Work item field values keyed by reference name\",\n      \"properties\": {\n        \"System.Id\": {\"type\": \"integer\"},\n        \"System.Title\": {\"type\": \"string\"},\n        \"System.WorkItemType\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Work item type (Bug, Task, User Story, Epic, Feature, Test Case, etc.)\"\n        },\n        \"System.State\": {\n          \"type\": \"string\",\n          \"description\": \"Current workflow state\"\n        },\n        \"System.Reason\": {\"type\": \"string\"},\n        \"System.AssignedTo\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"displayName\": {\"type\": \"string\"},\n            \"id\": {\"type\": \"string\"},\n            \"uniqueName\": {\"type\": \"string\"},\n            \"imageUrl\": {\"type\": \"string\"}\n          }\n        },\n        \"System.CreatedDate\": {\"type\": \"string\", \"format\": \"date-time\"},\n        \"System.CreatedBy\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"displayName\": {\"type\": \"string\"},\n            \"uniqueName\": {\"type\": \"string\"}\n          }\n        },\n        \"System.ChangedDate\": {\"\
  type\": \"string\", \"format\": \"date-time\"},\n        \"System.TeamProject\": {\"type\": \"string\"},\n        \"System.AreaPath\": {\"type\": \"string\"},\n        \"System.IterationPath\": {\"type\": \"string\"},\n        \"System.Description\": {\"type\": \"string\"},\n        \"System.Tags\": {\"type\": \"string\"},\n        \"Microsoft.VSTS.Common.Priority\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 4\n        },\n        \"Microsoft.VSTS.Common.Severity\": {\n          \"type\": \"string\",\n          \"enum\": [\"1 - Critical\", \"2 - High\", \"3 - Medium\", \"4 - Low\"]\n        },\n        \"Microsoft.VSTS.Scheduling.StoryPoints\": {\n          \"type\": \"number\"\n        },\n        \"Microsoft.VSTS.Scheduling.RemainingWork\": {\n          \"type\": \"number\"\n        },\n        \"Microsoft.VSTS.Scheduling.CompletedWork\": {\n          \"type\": \"number\"\n        },\n        \"Microsoft.VSTS.Build.IntegrationBuild\": {\n\
  \          \"type\": \"string\"\n        },\n        \"System.BoardColumn\": {\"type\": \"string\"},\n        \"System.BoardLane\": {\"type\": \"string\"}\n      },\n      \"additionalProperties\": true\n    },\n    \"relations\": {\n      \"type\": \"array\",\n      \"description\": \"Links to related work items and artifacts\",\n      \"items\": {\n        \"$ref\": \"#/$defs/WorkItemRelation\"\n      }\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for the work item\"\n    }\n  },\n  \"$defs\": {\n    \"WorkItemRelation\": {\n      \"type\": \"object\",\n      \"required\": [\"rel\", \"url\"],\n      \"properties\": {\n        \"rel\": {\n          \"type\": \"string\",\n          \"description\": \"Relation type reference name\",\n          \"examples\": [\n            \"System.LinkTypes.Hierarchy-Forward\",\n            \"System.LinkTypes.Hierarchy-Reverse\",\n            \"System.LinkTypes.Related\",\n          \
  \  \"System.LinkTypes.Duplicate-Forward\",\n            \"Microsoft.VSTS.TestCase.SharedParameterReferencedBy\"\n          ]\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"attributes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\"type\": \"string\"},\n            \"comment\": {\"type\": \"string\"},\n            \"isLocked\": {\"type\": \"boolean\"}\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-workitem-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
title: Azure DevOps Work Item
---
