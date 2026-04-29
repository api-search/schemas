---
description: ListDataQualityResultsResponse schema from Amazon Glue API
layout: schema
name: ListDataQualityResultsResponse
properties_list:
- description: ''
  name: Results
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-data-quality-results-response-schema.json
slug: glue-list-data-quality-results-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-data-quality-results-response-schema.json\",\n  \"title\": \"ListDataQualityResultsResponse\",\n  \"description\": \"ListDataQualityResultsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Results\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityResultDescriptionList\"\n        },\n        {\n          \"description\": \"A list of <code>DataQualityResultDescription</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A pagination token, if more results are available.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-data-quality-results-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListDataQualityResultsResponse
---
