---
description: A list of the pipelines associated with the current AWS account.
layout: schema
name: ListPipelinesResponse
properties_list:
- description: ''
  name: Pipelines
  type: object
- description: ''
  name: NextPageToken
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-list-pipelines-response-schema.json
slug: amazon-elastic-transcoder-list-pipelines-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-list-pipelines-response-schema.json\",\n  \"title\": \"ListPipelinesResponse\",\n  \"description\": \"A list of the pipelines associated with the current AWS account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Pipelines\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Pipelines\"\n        },\n        {\n          \"description\": \"An array of <code>Pipeline</code> objects.\"\n        }\n      ]\n    },\n    \"NextPageToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"A value that you use to access the second and subsequent pages of results, if any. When the pipelines fit on one page or when you've reached the last page of results,\
  \ the value of <code>NextPageToken</code> is <code>null</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-list-pipelines-response-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: ListPipelinesResponse
---
