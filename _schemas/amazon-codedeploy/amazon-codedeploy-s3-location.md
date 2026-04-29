---
description: Information about the location of application artifacts stored in Amazon S3.
layout: schema
name: S3Location
properties_list:
- description: ''
  name: bucket
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: bundleType
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: eTag
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-s3-location-schema.json
slug: amazon-codedeploy-s3-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-s3-location-schema.json\",\n  \"title\": \"S3Location\",\n  \"description\": \"Information about the location of application artifacts stored in Amazon S3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Bucket\"\n        },\n        {\n          \"description\": \"The name of the Amazon S3 bucket where the application revision is stored.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Key\"\n        },\n        {\n          \"description\": \"The name of the Amazon S3 object that represents the bundled artifacts for the application revision.\"\n        }\n      ]\n    },\n    \"bundleType\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/BundleType\"\n        },\n        {\n          \"description\": \"<p>The file type of the application revision. Must be one of the following:</p> <ul> <li> <p> <code>tar</code>: A tar archive file.</p> </li> <li> <p> <code>tgz</code>: A compressed tar archive file.</p> </li> <li> <p> <code>zip</code>: A zip archive file.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionId\"\n        },\n        {\n          \"description\": \"<p>A specific version of the Amazon S3 object that represents the bundled artifacts for the application revision.</p> <p>If the version is not specified, the system uses the most recent version by default.</p>\"\n        }\n      ]\n    },\n    \"eTag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ETag\"\n        },\n        {\n          \"description\": \"<p>The ETag of the Amazon\
  \ S3 object that represents the bundled artifacts for the application revision.</p> <p>If the ETag is not specified as an input parameter, ETag validation of the object is skipped.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-s3-location-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: S3Location
---
