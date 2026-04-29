---
description: Request to filter the contents of an Amazon S3 object based on a simple Structured Query Language (SQL) statement. In the request, along with the SQL expression, you must specify a data serialization format (JSON or CSV) of the object. Amazon S3 uses this to parse object data into records. It returns only records that match the specified SQL expression. You must also specify the data serialization format for the response. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTObjectSELECTContent.html">S3Select API Documentation</a>.
layout: schema
name: SelectObjectContentRequest
properties_list:
- description: ''
  name: Expression
  type: object
- description: ''
  name: ExpressionType
  type: object
- description: ''
  name: RequestProgress
  type: object
- description: ''
  name: InputSerialization
  type: object
- description: ''
  name: OutputSerialization
  type: object
- description: ''
  name: ScanRange
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-selectobjectcontentrequest-schema.json
slug: s3-selectobjectcontentrequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SelectObjectContentRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Expression\": {},\n    \"ExpressionType\": {},\n    \"RequestProgress\": {},\n    \"InputSerialization\": {},\n    \"OutputSerialization\": {},\n    \"ScanRange\": {}\n  },\n  \"required\": [\n    \"Expression\",\n    \"ExpressionType\",\n    \"InputSerialization\",\n    \"OutputSerialization\"\n  ],\n  \"description\": \"Request to filter the contents of an Amazon S3 object based on a simple Structured Query Language (SQL) statement. In the request, along with the SQL expression, you must specify a data serialization format (JSON or CSV) of the object. Amazon S3 uses this to parse object data into records. It returns only records that match the specified SQL expression. You must also specify the data serialization format for the response. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/RESTObjectSELECTContent.html\\\
  \">S3Select API Documentation</a>.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-selectobjectcontentrequest-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: SelectObjectContentRequest
---
