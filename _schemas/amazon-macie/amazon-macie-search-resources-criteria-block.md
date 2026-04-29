---
description: Specifies property- and tag-based conditions that define filter criteria for including or excluding Amazon Web Services resources from the query results.
layout: schema
name: SearchResourcesCriteriaBlock
properties_list:
- description: ''
  name: and
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-search-resources-criteria-block-schema.json
slug: amazon-macie-search-resources-criteria-block
source_filename: amazon-macie-search-resources-criteria-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-search-resources-criteria-block-schema.json\",\n  \"title\": \"SearchResourcesCriteriaBlock\",\n  \"description\": \"Specifies property- and tag-based conditions that define filter criteria for including or excluding Amazon Web Services resources from the query results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"and\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSearchResourcesCriteria\"\n        },\n        {\n          \"description\": \"An array of objects, one for each property- or tag-based condition that includes or excludes resources from the query results. If you specify more than one condition, Amazon Macie uses AND logic to join the conditions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-search-resources-criteria-block-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SearchResourcesCriteriaBlock
---
