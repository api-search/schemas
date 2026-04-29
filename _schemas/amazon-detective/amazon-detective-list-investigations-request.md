---
description: Request to list investigations
layout: schema
name: ListInvestigationsRequest
properties_list:
- description: The ARN of the behavior graph.
  name: GraphArn
  type: string
- description: Lists the investigations for a behavior graph based on the maximum number of investigations in a page.
  name: NextToken
  type: string
- description: Lists the investigations for a behavior graph based on the total number of investigations.
  name: MaxResults
  type: integer
- description: Filters the investigation results based on a criteria.
  name: FilterCriteria
  type: object
- description: Sorts the investigation results based on a criteria.
  name: SortCriteria
  type: object
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-investigations-request-schema.json
slug: amazon-detective-list-investigations-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-investigations-request-schema.json\",\n  \"title\": \"ListInvestigationsRequest\",\n  \"description\": \"Request to list investigations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Lists the investigations for a behavior graph based on the maximum number of investigations in a page.\",\n      \"example\": \"abc123token\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"Lists the investigations for a behavior graph based on the total number of investigations.\",\n \
  \     \"example\": 100\n    },\n    \"FilterCriteria\": {\n      \"type\": \"object\",\n      \"description\": \"Filters the investigation results based on a criteria.\",\n      \"properties\": {\n        \"Severity\": {\n          \"type\": \"object\",\n          \"description\": \"Filter investigations by severity.\",\n          \"properties\": {\n            \"Value\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"INFORMATIONAL\",\n                \"LOW\",\n                \"MEDIUM\",\n                \"HIGH\",\n                \"CRITICAL\"\n              ]\n            }\n          }\n        },\n        \"Status\": {\n          \"type\": \"object\",\n          \"description\": \"Filter investigations by status.\",\n          \"properties\": {\n            \"Value\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"RUNNING\",\n                \"FAILED\",\n                \"SUCCESSFUL\"\n              ]\n   \
  \         }\n          }\n        },\n        \"State\": {\n          \"type\": \"object\",\n          \"description\": \"Filter investigations by state.\",\n          \"properties\": {\n            \"Value\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"ACTIVE\",\n                \"ARCHIVED\"\n              ]\n            }\n          }\n        }\n      }\n    },\n    \"SortCriteria\": {\n      \"type\": \"object\",\n      \"description\": \"Sorts the investigation results based on a criteria.\",\n      \"properties\": {\n        \"Field\": {\n          \"type\": \"string\",\n          \"description\": \"The field to use to sort the results.\",\n          \"enum\": [\n            \"SEVERITY\",\n            \"STATUS\",\n            \"CREATED_TIME\"\n          ]\n        },\n        \"SortOrder\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ASC\",\n            \"DESC\"\n          ]\n        }\n      }\n    }\n  },\n \
  \ \"required\": [\n    \"GraphArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-investigations-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: ListInvestigationsRequest
---
