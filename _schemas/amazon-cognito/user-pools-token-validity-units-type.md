---
description: The data type TokenValidityUnits specifies the time units you use when you set the duration of ID, access, and refresh tokens.
layout: schema
name: TokenValidityUnitsType
properties_list:
- description: ''
  name: AccessToken
  type: object
- description: ''
  name: IdToken
  type: object
- description: ''
  name: RefreshToken
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-token-validity-units-type-schema.json
slug: user-pools-token-validity-units-type
source_filename: user-pools-token-validity-units-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-token-validity-units-type-schema.json\",\n  \"title\": \"TokenValidityUnitsType\",\n  \"description\": \"The data type TokenValidityUnits specifies the time units you use when you set the duration of ID, access, and refresh tokens.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeUnitsType\"\n        },\n        {\n          \"description\": \" A time unit of <code>seconds</code>, <code>minutes</code>, <code>hours</code>, or <code>days</code> for the value that you set in the <code>AccessTokenValidity</code> parameter. The default <code>AccessTokenValidity</code> time unit is hours. <code>AccessTokenValidity</code> duration can range from five minutes to one day.\"\n        }\n      ]\n    },\n\
  \    \"IdToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeUnitsType\"\n        },\n        {\n          \"description\": \"A time unit of <code>seconds</code>, <code>minutes</code>, <code>hours</code>, or <code>days</code> for the value that you set in the <code>IdTokenValidity</code> parameter. The default <code>IdTokenValidity</code> time unit is hours. <code>IdTokenValidity</code> duration can range from five minutes to one day.\"\n        }\n      ]\n    },\n    \"RefreshToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeUnitsType\"\n        },\n        {\n          \"description\": \"A time unit of <code>seconds</code>, <code>minutes</code>, <code>hours</code>, or <code>days</code> for the value that you set in the <code>RefreshTokenValidity</code> parameter. The default <code>RefreshTokenValidity</code> time unit is days. <code>RefreshTokenValidity</code> duration can range from 60 minutes to 10 years.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-token-validity-units-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: TokenValidityUnitsType
---
