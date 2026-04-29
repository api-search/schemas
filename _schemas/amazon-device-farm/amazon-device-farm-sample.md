---
description: Represents a sample of performance data.
layout: schema
name: Sample
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: url
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-sample-schema.json
slug: amazon-device-farm-sample
source_filename: amazon-device-farm-sample-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-sample-schema.json\",\n  \"title\": \"Sample\",\n  \"description\": \"Represents a sample of performance data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The sample's ARN.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleType\"\n        },\n        {\n          \"description\": \"<p>The sample's type.</p> <p>Must be one of the following values:</p> <ul> <li> <p>CPU: A CPU sample type. This is expressed as the app processing CPU time (including child processes) as reported by process, as a percentage.</p> </li> <li> <p>MEMORY: A memory\
  \ usage sample type. This is expressed as the total proportional set size of an app process, in kilobytes.</p> </li> <li> <p>NATIVE_AVG_DRAWTIME</p> </li> <li> <p>NATIVE_FPS</p> </li> <li> <p>NATIVE_FRAMES</p> </li> <li> <p>NATIVE_MAX_DRAWTIME</p> </li> <li> <p>NATIVE_MIN_DRAWTIME</p> </li> <li> <p>OPENGL_AVG_DRAWTIME</p> </li> <li> <p>OPENGL_FPS</p> </li> <li> <p>OPENGL_FRAMES</p> </li> <li> <p>OPENGL_MAX_DRAWTIME</p> </li> <li> <p>OPENGL_MIN_DRAWTIME</p> </li> <li> <p>RX</p> </li> <li> <p>RX_RATE: The total number of bytes per second (TCP and UDP) that are sent, by app process.</p> </li> <li> <p>THREADS: A threads sample type. This is expressed as the total number of threads per app process.</p> </li> <li> <p>TX</p> </li> <li> <p>TX_RATE: The total number of bytes per second (TCP and UDP) that are received, by app process.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/URL\"\n        },\n      \
  \  {\n          \"description\": \"The presigned Amazon S3 URL that can be used with a GET request to download the sample's file.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-sample-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: Sample
---
