---
description: Response for describing environments.
layout: schema
name: DescribeEnvironmentsResponse
properties_list:
- description: ''
  name: environments
  type: array
provider_name: Amazon Cloud9
provider_slug: amazon-cloud9
schema_file: json-schema/cloud9-describe-environments-response-schema.json
slug: cloud9-describe-environments-response
source_filename: cloud9-describe-environments-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud9/refs/heads/main/json-schema/cloud9-describe-environments-response-schema.json\",\n  \"title\": \"DescribeEnvironmentsResponse\",\n  \"description\": \"Response for describing environments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Environment\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud9/refs/heads/main/json-schema/cloud9-describe-environments-response-schema.json
tags:
- AWS
- Cloud9
- IDE
- Development
- Browser-Based
title: DescribeEnvironmentsResponse
---
