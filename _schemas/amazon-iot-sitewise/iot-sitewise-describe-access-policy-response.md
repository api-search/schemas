---
description: DescribeAccessPolicyResponse schema
layout: schema
name: DescribeAccessPolicyResponse
properties_list:
- description: ''
  name: accessPolicyId
  type: object
- description: ''
  name: accessPolicyArn
  type: object
- description: ''
  name: accessPolicyIdentity
  type: object
- description: ''
  name: accessPolicyResource
  type: object
- description: ''
  name: accessPolicyPermission
  type: object
- description: ''
  name: accessPolicyCreationDate
  type: object
- description: ''
  name: accessPolicyLastUpdateDate
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-describe-access-policy-response-schema.json
slug: iot-sitewise-describe-access-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-access-policy-response-schema.json\",\n  \"title\": \"DescribeAccessPolicyResponse\",\n  \"description\": \"DescribeAccessPolicyResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessPolicyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the access policy.\"\n        }\n      ]\n    },\n    \"accessPolicyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the access policy, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:access-policy/${AccessPolicyId}</code>\
  \ </p>\"\n        }\n      ]\n    },\n    \"accessPolicyIdentity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identity\"\n        },\n        {\n          \"description\": \"The identity (IAM Identity Center user, IAM Identity Center group, or IAM user) to which this access policy applies.\"\n        }\n      ]\n    },\n    \"accessPolicyResource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Resource\"\n        },\n        {\n          \"description\": \"The IoT SiteWise Monitor resource (portal or project) to which this access policy provides access.\"\n        }\n      ]\n    },\n    \"accessPolicyPermission\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Permission\"\n        },\n        {\n          \"description\": \"The access policy permission. Note that a project <code>ADMINISTRATOR</code> is also known as a project owner.\"\n        }\n      ]\n    },\n    \"accessPolicyCreationDate\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the access policy was created, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"accessPolicyLastUpdateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the access policy was last updated, in Unix epoch time.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accessPolicyId\",\n    \"accessPolicyArn\",\n    \"accessPolicyIdentity\",\n    \"accessPolicyResource\",\n    \"accessPolicyPermission\",\n    \"accessPolicyCreationDate\",\n    \"accessPolicyLastUpdateDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-access-policy-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DescribeAccessPolicyResponse
---
