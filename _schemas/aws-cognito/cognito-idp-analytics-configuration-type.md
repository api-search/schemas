---
description: <p>The Amazon Pinpoint analytics configuration necessary to collect metrics for a user pool.</p> <note> <p>In Regions where Amazon Pinpointisn't available, user pools only support sending events to Amazon Pinpoint projects in us-east-1. In Regions where Amazon Pinpoint is available, user pools support sending events to Amazon Pinpoint projects within that same Region.</p> </note>
layout: schema
name: AnalyticsConfigurationType
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: ApplicationArn
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: ExternalId
  type: object
- description: ''
  name: UserDataShared
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-analytics-configuration-type-schema.json
slug: cognito-idp-analytics-configuration-type
source_filename: cognito-idp-analytics-configuration-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HexStringType\"\n        },\n        {\n          \"description\": \"The application ID for an Amazon Pinpoint application.\"\n        }\n      ]\n    },\n    \"ApplicationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an Amazon Pinpoint project. You can use the Amazon Pinpoint project to integrate with the chosen user pool Client. Amazon Cognito publishes events to the Amazon Pinpoint project that the app ARN declares.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The ARN of an Identity and Access Management role that authorizes Amazon Cognito to publish events\
  \ to Amazon Pinpoint analytics.\"\n        }\n      ]\n    },\n    \"ExternalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The external ID.\"\n        }\n      ]\n    },\n    \"UserDataShared\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"If <code>UserDataShared</code> is <code>true</code>, Amazon Cognito includes user data in the events that it publishes to Amazon Pinpoint analytics.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p>The Amazon Pinpoint analytics configuration necessary to collect metrics for a user pool.</p> <note> <p>In Regions where Amazon Pinpointisn't available, user pools only support sending events to Amazon Pinpoint projects in us-east-1. In Regions where Amazon Pinpoint is available, user pools support sending events to Amazon Pinpoint projects within\
  \ that same Region.</p> </note>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-analytics-configuration-type-schema.json\",\n  \"title\": \"AnalyticsConfigurationType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-analytics-configuration-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AnalyticsConfigurationType
---
