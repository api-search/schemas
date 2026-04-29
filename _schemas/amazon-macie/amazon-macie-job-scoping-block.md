---
description: Specifies one or more property- and tag-based conditions that define criteria for including or excluding S3 objects from a classification job.
layout: schema
name: JobScopingBlock
properties_list:
- description: ''
  name: and
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-job-scoping-block-schema.json
slug: amazon-macie-job-scoping-block
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-job-scoping-block-schema.json\",\n  \"title\": \"JobScopingBlock\",\n  \"description\": \"Specifies one or more property- and tag-based conditions that define criteria for including or excluding S3 objects from a classification job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"and\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfJobScopeTerm\"\n        },\n        {\n          \"description\": \"An array of conditions, one for each property- or tag-based condition that determines which objects to include or exclude from the job. If you specify more than one condition, Amazon Macie uses AND logic to join the conditions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-job-scoping-block-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: JobScopingBlock
---
