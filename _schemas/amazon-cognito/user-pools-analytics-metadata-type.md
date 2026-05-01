---
description: <p>An Amazon Pinpoint analytics endpoint.</p> <p>An endpoint uniquely identifies a mobile device, email address, or phone number that can receive messages from Amazon Pinpoint analytics. For more information about Amazon Web Services Regions that can contain Amazon Pinpoint resources for use with Amazon Cognito user pools, see <a href="https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-pinpoint-integration.html">Using Amazon Pinpoint analytics with Amazon Cognito user pools</a>.</p>
layout: schema
name: AnalyticsMetadataType
properties_list:
- description: ''
  name: AnalyticsEndpointId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-analytics-metadata-type-schema.json
slug: user-pools-analytics-metadata-type
source_filename: user-pools-analytics-metadata-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-analytics-metadata-type-schema.json\",\n  \"title\": \"AnalyticsMetadataType\",\n  \"description\": \"<p>An Amazon Pinpoint analytics endpoint.</p> <p>An endpoint uniquely identifies a mobile device, email address, or phone number that can receive messages from Amazon Pinpoint analytics. For more information about Amazon Web Services Regions that can contain Amazon Pinpoint resources for use with Amazon Cognito user pools, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-pinpoint-integration.html\\\">Using Amazon Pinpoint analytics with Amazon Cognito user pools</a>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnalyticsEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n\
  \        {\n          \"description\": \"The endpoint ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-analytics-metadata-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: AnalyticsMetadataType
---
