---
description: <p>The device-remembering configuration for a user pool. A <a href="https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_DescribeUserPool.html"> DescribeUserPool</a> request returns a null value for this object when the user pool isn't configured to remember devices. When device remembering is active, you can remember a user's device with a <a href="https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_ConfirmDevice.html">ConfirmDevice</a> API request. Additionally. when the property <code>DeviceOnlyRememberedOnUserPrompt</code> is <code>true</code>, you must follow <code>ConfirmDevice</code> with an <a href="https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_UpdateDeviceStatus.html">UpdateDeviceStatus</a> API request that sets the user's device to <code>remembered</code> or <code>not_remembered</code>.</p> <p>To sign in with a remembered device, include <code>DEVICE_KEY</code> in the authentication
  parameters in your user's <a href="https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_InitiateAuth.html"> InitiateAuth</a> request. If your app doesn't include a <code>DEVICE_KEY</code> parameter, the <a href="https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_InitiateAuth.html#API_InitiateAuth_ResponseSyntax">response</a> from Amazon Cognito includes newly-generated <code>DEVICE_KEY</code> and <code>DEVICE_GROUP_KEY</code> values under <code>NewDeviceMetadata</code>. Store these values to use in future device-authentication requests.</p> <note> <p>When you provide a value for any property of <code>DeviceConfiguration</code>, you activate the device remembering for the user pool.</p> </note>
layout: schema
name: DeviceConfigurationType
properties_list:
- description: ''
  name: ChallengeRequiredOnNewDevice
  type: object
- description: ''
  name: DeviceOnlyRememberedOnUserPrompt
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-device-configuration-type-schema.json
slug: cognito-idp-device-configuration-type
source_filename: cognito-idp-device-configuration-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChallengeRequiredOnNewDevice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"<p>When true, a remembered device can sign in with device authentication instead of SMS and time-based one-time password (TOTP) factors for multi-factor authentication (MFA).</p> <note> <p>Whether or not <code>ChallengeRequiredOnNewDevice</code> is true, users who sign in with devices that have not been confirmed or remembered must still provide a second factor in a user pool that requires MFA.</p> </note>\"\n        }\n      ]\n    },\n    \"DeviceOnlyRememberedOnUserPrompt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"<p>When true, Amazon Cognito doesn't automatically remember a user's device when your app sends a <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_ConfirmDevice.html\\\
  \"> ConfirmDevice</a> API request. In your app, create a prompt for your user to choose whether they want to remember their device. Return the user's choice in an <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_UpdateDeviceStatus.html\\\"> UpdateDeviceStatus</a> API request.</p> <p>When <code>DeviceOnlyRememberedOnUserPrompt</code> is <code>false</code>, Amazon Cognito immediately remembers devices that you register in a <code>ConfirmDevice</code> API request.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p>The device-remembering configuration for a user pool. A <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_DescribeUserPool.html\\\"> DescribeUserPool</a> request returns a null value for this object when the user pool isn't configured to remember devices. When device remembering is active, you can remember a user's device with a <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_ConfirmDevice.html\\\
  \">ConfirmDevice</a> API request. Additionally. when the property <code>DeviceOnlyRememberedOnUserPrompt</code> is <code>true</code>, you must follow <code>ConfirmDevice</code> with an <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_UpdateDeviceStatus.html\\\">UpdateDeviceStatus</a> API request that sets the user's device to <code>remembered</code> or <code>not_remembered</code>.</p> <p>To sign in with a remembered device, include <code>DEVICE_KEY</code> in the authentication parameters in your user's <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_InitiateAuth.html\\\"> InitiateAuth</a> request. If your app doesn't include a <code>DEVICE_KEY</code> parameter, the <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_InitiateAuth.html#API_InitiateAuth_ResponseSyntax\\\">response</a> from Amazon Cognito includes newly-generated <code>DEVICE_KEY</code> and <code>DEVICE_GROUP_KEY</code>\
  \ values under <code>NewDeviceMetadata</code>. Store these values to use in future device-authentication requests.</p> <note> <p>When you provide a value for any property of <code>DeviceConfiguration</code>, you activate the device remembering for the user pool.</p> </note>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-device-configuration-type-schema.json\",\n  \"title\": \"DeviceConfigurationType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-device-configuration-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DeviceConfigurationType
---
