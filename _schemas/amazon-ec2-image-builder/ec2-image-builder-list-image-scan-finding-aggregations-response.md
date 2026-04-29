---
description: ListImageScanFindingAggregationsResponse schema from EC2 Image Builder
layout: schema
name: ListImageScanFindingAggregationsResponse
properties_list:
- description: ''
  name: requestId
  type: object
- description: ''
  name: aggregationType
  type: object
- description: ''
  name: responses
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-list-image-scan-finding-aggregations-response-schema.json
slug: ec2-image-builder-list-image-scan-finding-aggregations-response
source_filename: ec2-image-builder-list-image-scan-finding-aggregations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-scan-finding-aggregations-response-schema.json\",\n  \"title\": \"ListImageScanFindingAggregationsResponse\",\n  \"description\": \"ListImageScanFindingAggregationsResponse schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The request ID that uniquely identifies this request.\"\n        }\n      ]\n    },\n    \"aggregationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The aggregation type specifies what type of key is used to group the image scan findings. Image\
  \ Builder returns results based on the request filter. If you didn't specify a filter in the request, the type defaults to <code>accountId</code>.</p> <p class=\\\"title\\\"> <b>Aggregation types</b> </p> <ul> <li> <p>accountId</p> </li> <li> <p>imageBuildVersionArn</p> </li> <li> <p>imagePipelineArn</p> </li> <li> <p>vulnerabilityId</p> </li> </ul> <p>Each aggregation includes counts by severity level for medium severity and higher level findings, plus a total for all of the findings for each key value.</p>\"\n        }\n      ]\n    },\n    \"responses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageScanFindingAggregationsList\"\n        },\n        {\n          \"description\": \"An array of image scan finding aggregations that match the filter criteria.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\"\
  : \"The next token used for paginated responses. When this field isn't empty, there are additional elements that the service has'ot included in this request. Use this token with the next request to retrieve additional objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-scan-finding-aggregations-response-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListImageScanFindingAggregationsResponse
---
