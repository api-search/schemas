---
description: A location in Amazon Simple Storage Service (Amazon S3) where SimSpace Weaver stores simulation data, such as your app .zip files and schema file. For more information about Amazon S3, see the <a href="https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html"> <i>Amazon Simple Storage Service User Guide</i> </a>.
layout: schema
name: S3Location
properties_list:
- description: ''
  name: BucketName
  type: object
- description: ''
  name: ObjectKey
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-s3-location-schema.json
slug: amazon-simspace-weaver-s3-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-s3-location-schema.json\",\n  \"title\": \"S3Location\",\n  \"description\": \"A location in Amazon Simple Storage Service (Amazon S3) where SimSpace Weaver stores simulation data, such as your app .zip files and schema file. For more information about Amazon S3, see the <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html\\\"> <i>Amazon Simple Storage Service User Guide</i> </a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketName\"\n        },\n        {\n          \"description\": \"The name of an Amazon S3 bucket. For more information about buckets, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-buckets-s3.html\\\
  \">Creating, configuring, and working with Amazon S3 buckets</a> in the <i>Amazon Simple Storage Service User Guide</i>.\"\n        }\n      ]\n    },\n    \"ObjectKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectKey\"\n        },\n        {\n          \"description\": \"The key name of an object in Amazon S3. For more information about Amazon S3 objects and object keys, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/uploading-downloading-objects.html\\\">Uploading, downloading, and working with objects in Amazon S3</a> in the <i>Amazon Simple Storage Service User Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-s3-location-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: S3Location
---
