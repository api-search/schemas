---
description: Information about a data source.
layout: schema
name: DataSource
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: s3Bucket
  type: object
- description: ''
  name: s3Keys
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: destination
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-data-source-schema.json
slug: amazon-robomaker-openapi-data-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-data-source-schema.json\",\n  \"title\": \"DataSource\",\n  \"description\": \"Information about a data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the data source.\"\n        }\n      ]\n    },\n    \"s3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Bucket\"\n        },\n        {\n          \"description\": \"The S3 bucket where the data files are located.\"\n        }\n      ]\n    },\n    \"s3Keys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3KeyOutputs\"\n        },\n        {\n          \"description\": \"The list of S3\
  \ keys identifying the data source files.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceType\"\n        },\n        {\n          \"description\": \"<p>The data type for the data source that you're using for your container image or simulation job. You can use this field to specify whether your data source is an Archive, an Amazon S3 prefix, or a file.</p> <p>If you don't specify a field, the default value is <code>File</code>.</p>\"\n        }\n      ]\n    },\n    \"destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Path\"\n        },\n        {\n          \"description\": \"<p>The location where your files are mounted in the container image.</p> <p>If you've specified the <code>type</code> of the data source as an <code>Archive</code>, you must provide an Amazon S3 object key to your archive. The object key must point to either a <code>.zip</code> or <code>.tar.gz</code>\
  \ file.</p> <p>If you've specified the <code>type</code> of the data source as a <code>Prefix</code>, you provide the Amazon S3 prefix that points to the files that you are using for your data source.</p> <p>If you've specified the <code>type</code> of the data source as a <code>File</code>, you provide the Amazon S3 path to the file that you're using as your data source.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-data-source-schema.json
tags:
- AWS
- Robotics
- Simulation
title: DataSource
---
