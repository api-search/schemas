---
description: Each <code>S3Resource</code> object represents an Amazon S3 bucket that your transferred data will be exported from or imported into. For export jobs, this object can have an optional <code>KeyRange</code> value. The length of the range is defined at job creation, and has either an inclusive <code>BeginMarker</code>, an inclusive <code>EndMarker</code>, or both. Ranges are UTF-8 binary sorted.
layout: schema
name: S3Resource
properties_list:
- description: ''
  name: BucketArn
  type: object
- description: ''
  name: KeyRange
  type: object
- description: ''
  name: TargetOnDeviceServices
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-s3-resource-schema.json
slug: amazon-snow-family-s3-resource
source_filename: amazon-snow-family-s3-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-s3-resource-schema.json\",\n  \"title\": \"S3Resource\",\n  \"description\": \"Each <code>S3Resource</code> object represents an Amazon S3 bucket that your transferred data will be exported from or imported into. For export jobs, this object can have an optional <code>KeyRange</code> value. The length of the range is defined at job creation, and has either an inclusive <code>BeginMarker</code>, an inclusive <code>EndMarker</code>, or both. Ranges are UTF-8 binary sorted.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an Amazon S3 bucket.\"\n        }\n      ]\n    },\n    \"KeyRange\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyRange\"\n        },\n        {\n          \"description\": \"For export jobs, you can provide an optional <code>KeyRange</code> within a specific Amazon S3 bucket. The length of the range is defined at job creation, and has either an inclusive <code>BeginMarker</code>, an inclusive <code>EndMarker</code>, or both. Ranges are UTF-8 binary sorted.\"\n        }\n      ]\n    },\n    \"TargetOnDeviceServices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetOnDeviceServiceList\"\n        },\n        {\n          \"description\": \"Specifies the service or services on the Snow Family device that your transferred data will be exported from or imported into. Amazon Web Services Snow Family supports Amazon S3 and NFS (Network File System).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-s3-resource-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: S3Resource
---
