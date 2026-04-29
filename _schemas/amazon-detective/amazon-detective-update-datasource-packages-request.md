---
description: Request to update datasource packages for a behavior graph
layout: schema
name: UpdateDatasourcePackagesRequest
properties_list:
- description: The ARN of the behavior graph.
  name: GraphArn
  type: string
- description: The data source package start for the behavior graph.
  name: DatasourcePackages
  type: array
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-update-datasource-packages-request-schema.json
slug: amazon-detective-update-datasource-packages-request
source_filename: amazon-detective-update-datasource-packages-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-update-datasource-packages-request-schema.json\",\n  \"title\": \"UpdateDatasourcePackagesRequest\",\n  \"description\": \"Request to update datasource packages for a behavior graph\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"DatasourcePackages\": {\n      \"type\": \"array\",\n      \"description\": \"The data source package start for the behavior graph.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"DETECTIVE_CORE\",\n          \"EKS_AUDIT\",\n          \"AD_AUDIT\"\n        ]\n      },\n      \"example\": [\n        \"EKS_AUDIT\"\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"GraphArn\",\n    \"DatasourcePackages\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-update-datasource-packages-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: UpdateDatasourcePackagesRequest
---
