---
description: DescribePortalResponse schema
layout: schema
name: DescribePortalResponse
properties_list:
- description: ''
  name: portalId
  type: object
- description: ''
  name: portalArn
  type: object
- description: ''
  name: portalName
  type: object
- description: ''
  name: portalDescription
  type: object
- description: ''
  name: portalClientId
  type: object
- description: ''
  name: portalStartUrl
  type: object
- description: ''
  name: portalContactEmail
  type: object
- description: ''
  name: portalStatus
  type: object
- description: ''
  name: portalCreationDate
  type: object
- description: ''
  name: portalLastUpdateDate
  type: object
- description: ''
  name: portalLogoImageLocation
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: portalAuthMode
  type: object
- description: ''
  name: notificationSenderEmail
  type: object
- description: ''
  name: alarms
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-describe-portal-response-schema.json
slug: iot-sitewise-describe-portal-response
source_filename: iot-sitewise-describe-portal-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-portal-response-schema.json\",\n  \"title\": \"DescribePortalResponse\",\n  \"description\": \"DescribePortalResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the portal.\"\n        }\n      ]\n    },\n    \"portalArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the portal, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:portal/${PortalId}</code> </p>\"\n\
  \        }\n      ]\n    },\n    \"portalName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the portal.\"\n        }\n      ]\n    },\n    \"portalDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The portal's description.\"\n        }\n      ]\n    },\n    \"portalClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortalClientId\"\n        },\n        {\n          \"description\": \"The IAM Identity Center application generated client ID (used with IAM Identity Center APIs). IoT SiteWise includes <code>portalClientId</code> for only portals that use IAM Identity Center to authenticate users.\"\n        }\n      ]\n    },\n    \"portalStartUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n       \
  \ },\n        {\n          \"description\": \"The URL for the IoT SiteWise Monitor portal. You can use this URL to access portals that use IAM Identity Center for authentication. For portals that use IAM for authentication, you must use the IoT SiteWise console to get a URL that you can use to access the portal.\"\n        }\n      ]\n    },\n    \"portalContactEmail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Email\"\n        },\n        {\n          \"description\": \"The Amazon Web Services administrator's contact email address.\"\n        }\n      ]\n    },\n    \"portalStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortalStatus\"\n        },\n        {\n          \"description\": \"The current status of the portal, which contains a state and any error message.\"\n        }\n      ]\n    },\n    \"portalCreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n\
  \        },\n        {\n          \"description\": \"The date the portal was created, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"portalLastUpdateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the portal was last updated, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"portalLogoImageLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageLocation\"\n        },\n        {\n          \"description\": \"The portal's logo image, which is available at a URL.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the service role that allows the portal's users to access your IoT SiteWise resources\
  \ on your behalf. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/monitor-service-role.html\\\">Using service roles for IoT SiteWise Monitor</a> in the <i>IoT SiteWise User Guide</i>.\"\n        }\n      ]\n    },\n    \"portalAuthMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthMode\"\n        },\n        {\n          \"description\": \"The service to use to authenticate users to the portal.\"\n        }\n      ]\n    },\n    \"notificationSenderEmail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Email\"\n        },\n        {\n          \"description\": \"The email address that sends alarm notifications.\"\n        }\n      ]\n    },\n    \"alarms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Alarms\"\n        },\n        {\n          \"description\": \"Contains the configuration information of an alarm created in an IoT SiteWise\
  \ Monitor portal.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"portalId\",\n    \"portalArn\",\n    \"portalName\",\n    \"portalClientId\",\n    \"portalStartUrl\",\n    \"portalContactEmail\",\n    \"portalStatus\",\n    \"portalCreationDate\",\n    \"portalLastUpdateDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-portal-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DescribePortalResponse
---
