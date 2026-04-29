---
description: The Amazon S3 bucket where the Amazon Web Services IoT FleetWise campaign sends data. Amazon S3 is an object storage service that stores data as objects within buckets. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-buckets-s3.html">Creating, configuring, and working with Amazon S3 buckets</a> in the <i>Amazon Simple Storage Service User Guide</i>.
layout: schema
name: S3Config
properties_list:
- description: ''
  name: bucketArn
  type: object
- description: ''
  name: dataFormat
  type: object
- description: ''
  name: storageCompressionFormat
  type: object
- description: ''
  name: prefix
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-s3-config-schema.json
slug: iot-fleetwise-s3-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-s3-config-schema.json\",\n  \"title\": \"S3Config\",\n  \"description\": \"The Amazon S3 bucket where the Amazon Web Services IoT FleetWise campaign sends data. Amazon S3 is an object storage service that stores data as objects within buckets. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-buckets-s3.html\\\">Creating, configuring, and working with Amazon S3 buckets</a> in the <i>Amazon Simple Storage Service User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Amazon S3 bucket.\"\n        }\n      ]\n    },\n    \"dataFormat\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataFormat\"\n        },\n        {\n          \"description\": \"<p>Specify the format that files are saved in the Amazon S3 bucket. You can save files in an Apache Parquet or JSON format.</p> <ul> <li> <p>Parquet - Store data in a columnar storage file format. Parquet is optimal for fast data retrieval and can reduce costs. This option is selected by default.</p> </li> <li> <p>JSON - Store data in a standard text-based JSON file format.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"storageCompressionFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageCompressionFormat\"\n        },\n        {\n          \"description\": \"By default, stored data is compressed as a .gzip file. Compressed files have a reduced file size, which can optimize the cost of data storage.\"\n        }\n      ]\n    },\n    \"prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Prefix\"\n        },\n        {\n          \"description\": \"<p>(Optional) Enter an S3 bucket prefix. The prefix is the string of characters after the bucket name and before the object name. You can use the prefix to organize data stored in Amazon S3 buckets. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/using-prefixes.html\\\">Organizing objects using prefixes</a> in the <i>Amazon Simple Storage Service User Guide</i>.</p> <p>By default, Amazon Web Services IoT FleetWise sets the prefix <code>processed-data/year=YY/month=MM/date=DD/hour=HH/</code> (in UTC) to data it delivers to Amazon S3. You can enter a prefix to append it to this default prefix. For example, if you enter the prefix <code>vehicles</code>, the prefix will be <code>vehicles/processed-data/year=YY/month=MM/date=DD/hour=HH/</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bucketArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-s3-config-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: S3Config
---
