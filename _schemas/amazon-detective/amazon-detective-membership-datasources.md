---
description: Details on data source packages for a member account in a behavior graph
layout: schema
name: MembershipDatasources
properties_list:
- description: The account identifier of the AWS account.
  name: AccountId
  type: string
- description: The ARN of the organization behavior graph.
  name: GraphArn
  type: string
- description: Details on when a data source package was added to a behavior graph.
  name: DatasourcePackageIngestHistory
  type: object
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-membership-datasources-schema.json
slug: amazon-detective-membership-datasources
source_filename: amazon-detective-membership-datasources-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-membership-datasources-schema.json\",\n  \"title\": \"MembershipDatasources\",\n  \"description\": \"Details on data source packages for a member account in a behavior graph\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account identifier of the AWS account.\",\n      \"example\": \"234567890123\"\n    },\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the organization behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"DatasourcePackageIngestHistory\": {\n      \"type\": \"object\",\n      \"description\": \"Details on when a data source package was added to a behavior graph.\",\n      \"additionalProperties\"\
  : {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-membership-datasources-schema.json
tags:
- Forensics
- Investigation
- Security
title: MembershipDatasources
---
