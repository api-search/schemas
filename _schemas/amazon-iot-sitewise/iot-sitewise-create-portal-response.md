---
description: CreatePortalResponse schema
layout: schema
name: CreatePortalResponse
properties_list:
- description: ''
  name: portalId
  type: object
- description: ''
  name: portalArn
  type: object
- description: ''
  name: portalStartUrl
  type: object
- description: ''
  name: portalStatus
  type: object
- description: ''
  name: ssoApplicationId
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-create-portal-response-schema.json
slug: iot-sitewise-create-portal-response
source_filename: iot-sitewise-create-portal-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-portal-response-schema.json\",\n  \"title\": \"CreatePortalResponse\",\n  \"description\": \"CreatePortalResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the created portal.\"\n        }\n      ]\n    },\n    \"portalArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the portal, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:portal/${PortalId}</code> </p>\"\
  \n        }\n      ]\n    },\n    \"portalStartUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"The URL for the IoT SiteWise Monitor portal. You can use this URL to access portals that use IAM Identity Center for authentication. For portals that use IAM for authentication, you must use the IoT SiteWise console to get a URL that you can use to access the portal.\"\n        }\n      ]\n    },\n    \"portalStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortalStatus\"\n        },\n        {\n          \"description\": \"The status of the portal, which contains a state (<code>CREATING</code> after successfully calling this operation) and any error message.\"\n        }\n      ]\n    },\n    \"ssoApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SSOApplicationId\"\n        },\n        {\n          \"description\": \"\
  The associated IAM Identity Center application ID, if the portal uses IAM Identity Center.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"portalId\",\n    \"portalArn\",\n    \"portalStartUrl\",\n    \"portalStatus\",\n    \"ssoApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-portal-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: CreatePortalResponse
---
