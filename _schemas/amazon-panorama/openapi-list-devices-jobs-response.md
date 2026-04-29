---
description: ListDevicesJobsResponse schema from Amazon Panorama
layout: schema
name: ListDevicesJobsResponse
properties_list:
- description: ''
  name: DeviceJobs
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-list-devices-jobs-response-schema.json
slug: openapi-list-devices-jobs-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-list-devices-jobs-response-schema.json\",\n  \"title\": \"ListDevicesJobsResponse\",\n  \"description\": \"ListDevicesJobsResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeviceJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceJobList\"\n        },\n        {\n          \"description\": \"A list of jobs.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token that's included if more results are available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-list-devices-jobs-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: ListDevicesJobsResponse
---
