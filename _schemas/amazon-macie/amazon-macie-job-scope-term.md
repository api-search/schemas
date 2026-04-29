---
description: Specifies a property- or tag-based condition that defines criteria for including or excluding S3 objects from a classification job. A JobScopeTerm object can contain only one simpleScopeTerm object or one tagScopeTerm object.
layout: schema
name: JobScopeTerm
properties_list:
- description: ''
  name: simpleScopeTerm
  type: object
- description: ''
  name: tagScopeTerm
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-job-scope-term-schema.json
slug: amazon-macie-job-scope-term
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-job-scope-term-schema.json\",\n  \"title\": \"JobScopeTerm\",\n  \"description\": \"Specifies a property- or tag-based condition that defines criteria for including or excluding S3 objects from a classification job. A JobScopeTerm object can contain only one simpleScopeTerm object or one tagScopeTerm object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"simpleScopeTerm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimpleScopeTerm\"\n        },\n        {\n          \"description\": \"A property-based condition that defines a property, operator, and one or more values for including or excluding objects from the job.\"\n        }\n      ]\n    },\n    \"tagScopeTerm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagScopeTerm\"\
  \n        },\n        {\n          \"description\": \"A tag-based condition that defines the operator and tag keys or tag key and value pairs for including or excluding objects from the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-job-scope-term-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: JobScopeTerm
---
