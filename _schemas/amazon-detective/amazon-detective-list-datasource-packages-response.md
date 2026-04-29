---
description: Response from listing datasource packages
layout: schema
name: ListDatasourcePackagesResponse
properties_list:
- description: Details on the data source packages active in the behavior graph.
  name: DatasourcePackages
  type: object
- description: For requests to get the next page of results.
  name: NextToken
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-datasource-packages-response-schema.json
slug: amazon-detective-list-datasource-packages-response
source_filename: amazon-detective-list-datasource-packages-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-datasource-packages-response-schema.json\",\n  \"title\": \"ListDatasourcePackagesResponse\",\n  \"description\": \"Response from listing datasource packages\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasourcePackages\": {\n      \"type\": \"object\",\n      \"description\": \"Details on the data source packages active in the behavior graph.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/DatasourcePackageIngestDetail\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"For requests to get the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-datasource-packages-response-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: ListDatasourcePackagesResponse
---
