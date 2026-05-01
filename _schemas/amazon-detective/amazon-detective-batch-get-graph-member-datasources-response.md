---
description: Response from getting datasource details for behavior graph members
layout: schema
name: BatchGetGraphMemberDatasourcesResponse
properties_list:
- description: Details on the data source packages active in the behavior graph.
  name: MemberDatasources
  type: array
- description: Accounts that data source package information could not be retrieved for.
  name: UnprocessedAccounts
  type: array
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-batch-get-graph-member-datasources-response-schema.json
slug: amazon-detective-batch-get-graph-member-datasources-response
source_filename: amazon-detective-batch-get-graph-member-datasources-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-batch-get-graph-member-datasources-response-schema.json\",\n  \"title\": \"BatchGetGraphMemberDatasourcesResponse\",\n  \"description\": \"Response from getting datasource details for behavior graph members\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MemberDatasources\": {\n      \"type\": \"array\",\n      \"description\": \"Details on the data source packages active in the behavior graph.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MembershipDatasources\"\n      }\n    },\n    \"UnprocessedAccounts\": {\n      \"type\": \"array\",\n      \"description\": \"Accounts that data source package information could not be retrieved for.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UnprocessedAccount\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-batch-get-graph-member-datasources-response-schema.json
tags:
- Forensics
- Investigation
- Security
title: BatchGetGraphMemberDatasourcesResponse
---
