---
description: Information about the location of an application revision.
layout: schema
name: RevisionLocation
properties_list:
- description: ''
  name: revisionType
  type: object
- description: ''
  name: s3Location
  type: object
- description: ''
  name: gitHubLocation
  type: object
- description: ''
  name: string
  type: object
- description: ''
  name: appSpecContent
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-revision-location-schema.json
slug: amazon-codedeploy-revision-location
source_filename: amazon-codedeploy-revision-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-revision-location-schema.json\",\n  \"title\": \"RevisionLocation\",\n  \"description\": \"Information about the location of an application revision.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revisionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionLocationType\"\n        },\n        {\n          \"description\": \"<p>The type of application revision:</p> <ul> <li> <p>S3: An application revision stored in Amazon S3.</p> </li> <li> <p>GitHub: An application revision stored in GitHub (EC2/On-premises deployments only).</p> </li> <li> <p>String: A YAML-formatted or JSON-formatted string (Lambda deployments only).</p> </li> <li> <p>AppSpecContent: An <code>AppSpecContent</code> object that contains the contents of an AppSpec file\
  \ for an Lambda or Amazon ECS deployment. The content is formatted as JSON or YAML stored as a RawString.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"s3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"Information about the location of a revision stored in Amazon S3. \"\n        }\n      ]\n    },\n    \"gitHubLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitHubLocation\"\n        },\n        {\n          \"description\": \"Information about the location of application artifacts stored in GitHub.\"\n        }\n      ]\n    },\n    \"string\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RawString\"\n        },\n        {\n          \"description\": \"Information about the location of an Lambda deployment revision stored as a RawString.\"\n        }\n      ]\n    },\n    \"appSpecContent\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AppSpecContent\"\n        },\n        {\n          \"description\": \" The content of an AppSpec file for an Lambda or Amazon ECS deployment. The content is formatted as JSON or YAML and stored as a RawString. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-revision-location-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: RevisionLocation
---
