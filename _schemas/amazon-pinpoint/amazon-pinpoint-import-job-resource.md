---
description: Provides information about the resource settings for a job that imports endpoint definitions from one or more files. The files can be stored in an Amazon Simple Storage Service (Amazon S3) bucket or uploaded directly from a computer by using the Amazon Pinpoint console.
layout: schema
name: ImportJobResource
properties_list:
- description: ''
  name: DefineSegment
  type: object
- description: ''
  name: ExternalId
  type: object
- description: ''
  name: Format
  type: object
- description: ''
  name: RegisterEndpoints
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: S3Url
  type: object
- description: ''
  name: SegmentId
  type: object
- description: ''
  name: SegmentName
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-import-job-resource-schema.json
slug: amazon-pinpoint-import-job-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-import-job-resource-schema.json\",\n  \"title\": \"ImportJobResource\",\n  \"description\": \"Provides information about the resource settings for a job that imports endpoint definitions from one or more files. The files can be stored in an Amazon Simple Storage Service (Amazon S3) bucket or uploaded directly from a computer by using the Amazon Pinpoint console.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DefineSegment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the import job creates a segment that contains the endpoints, when the endpoint definitions are imported.\"\n        }\n      ]\n    },\n    \"ExternalId\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"(Deprecated) Your AWS account ID, which you assigned to an external ID key in an IAM trust policy. Amazon Pinpoint previously used this value to assume an IAM role when importing endpoint definitions, but we removed this requirement. We don't recommend use of external IDs for IAM roles that are assumed by Amazon Pinpoint.\"\n        }\n      ]\n    },\n    \"Format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Format\"\n        },\n        {\n          \"description\": \"<p>The format of the files that contain the endpoint definitions to import. Valid values are: CSV, for comma-separated values format; and, JSON, for newline-delimited JSON format.</p> <p>If the files are stored in an Amazon S3 location and that location contains multiple files that use different formats, Amazon Pinpoint imports data only from the files that use the specified format.</p>\"\
  \n        }\n      ]\n    },\n    \"RegisterEndpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the import job registers the endpoints with Amazon Pinpoint, when the endpoint definitions are imported.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the AWS Identity and Access Management (IAM) role that authorizes Amazon Pinpoint to access the Amazon S3 location to import endpoint definitions from.\"\n        }\n      ]\n    },\n    \"S3Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The URL of the Amazon Simple Storage Service (Amazon S3) bucket that contains the endpoint definitions to import.\
  \ This location can be a folder or a single file. If the location is a folder, Amazon Pinpoint imports endpoint definitions from the files in this location, including any subfolders that the folder contains.</p> <p>The URL should be in the following format: s3://<replaceable>bucket-name</replaceable>/<replaceable>folder-name</replaceable>/<replaceable>file-name</replaceable>. The location can end with the key for an individual object or a prefix that qualifies multiple objects.</p>\"\n        }\n      ]\n    },\n    \"SegmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The identifier for the segment that the import job updates or adds endpoint definitions to, if the import job updates an existing segment.\"\n        }\n      ]\n    },\n    \"SegmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\"\
  : \"The custom name for the segment that's created by the import job, if the value of the DefineSegment property is true.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Format\",\n    \"S3Url\",\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-import-job-resource-schema.json
tags:
- AWS
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: ImportJobResource
---
