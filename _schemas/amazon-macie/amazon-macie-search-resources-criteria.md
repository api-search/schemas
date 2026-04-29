---
description: Specifies a property- or tag-based filter condition for including or excluding Amazon Web Services resources from the query results.
layout: schema
name: SearchResourcesCriteria
properties_list:
- description: ''
  name: simpleCriterion
  type: object
- description: ''
  name: tagCriterion
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-search-resources-criteria-schema.json
slug: amazon-macie-search-resources-criteria
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-search-resources-criteria-schema.json\",\n  \"title\": \"SearchResourcesCriteria\",\n  \"description\": \"Specifies a property- or tag-based filter condition for including or excluding Amazon Web Services resources from the query results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"simpleCriterion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchResourcesSimpleCriterion\"\n        },\n        {\n          \"description\": \"A property-based condition that defines a property, operator, and one or more values for including or excluding resources from the results.\"\n        }\n      ]\n    },\n    \"tagCriterion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchResourcesTagCriterion\"\n        },\n        {\n \
  \         \"description\": \"A tag-based condition that defines an operator and tag keys, tag values, or tag key and value pairs for including or excluding resources from the results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-search-resources-criteria-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SearchResourcesCriteria
---
