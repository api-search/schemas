---
description: DescribeAuditSuppressionResponse schema
layout: schema
name: DescribeAuditSuppressionResponse
properties_list:
- description: An audit check name. Checks must be enabled for your account. (Use <code>DescribeAccountAuditConfiguration</code> to see the list of all checks, including those that are enabled or use <code>UpdateAcc
  name: checkName
  type: string
- description: Information that identifies the noncompliant resource.
  name: resourceIdentifier
  type: object
- description: ''
  name: expirationDate
  type: object
- description: ''
  name: suppressIndefinitely
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-audit-suppression-response-schema.json
slug: iot-device-management-describe-audit-suppression-response
source_filename: iot-device-management-describe-audit-suppression-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-audit-suppression-response-schema.json\",\n  \"title\": \"DescribeAuditSuppressionResponse\",\n  \"description\": \"DescribeAuditSuppressionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkName\": {\n      \"type\": \"string\",\n      \"description\": \"An audit check name. Checks must be enabled for your account. (Use <code>DescribeAccountAuditConfiguration</code> to see the list of all checks, including those that are enabled or use <code>UpdateAccountAuditConfiguration</code> to select which checks are enabled.)\"\n    },\n    \"resourceIdentifier\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"deviceCertificateId\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/CertificateId\"\
  \n            },\n            {\n              \"description\": \"The ID of the certificate attached to the resource.\"\n            }\n          ]\n        },\n        \"caCertificateId\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/CertificateId\"\n            },\n            {\n              \"description\": \"The ID of the CA certificate used to authorize the certificate.\"\n            }\n          ]\n        },\n        \"cognitoIdentityPoolId\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/CognitoIdentityPoolId\"\n            },\n            {\n              \"description\": \"The ID of the Amazon Cognito identity pool.\"\n            }\n          ]\n        },\n        \"clientId\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ClientId\"\n            },\n            {\n              \"description\": \"The client ID.\"\n            }\n          ]\n\
  \        },\n        \"policyVersionIdentifier\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/PolicyVersionIdentifier\"\n            },\n            {\n              \"description\": \"The version of the policy associated with the resource.\"\n            }\n          ]\n        },\n        \"account\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/AwsAccountId\"\n            },\n            {\n              \"description\": \"The account with which the resource is associated.\"\n            }\n          ]\n        },\n        \"iamRoleArn\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/RoleArn\"\n            },\n            {\n              \"description\": \"The ARN of the IAM role that has overly permissive actions.\"\n            }\n          ]\n        },\n        \"roleAliasArn\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/RoleAliasArn\"\
  \n            },\n            {\n              \"description\": \"The ARN of the role alias that has overly permissive actions.\"\n            }\n          ]\n        },\n        \"issuerCertificateIdentifier\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/IssuerCertificateIdentifier\"\n            },\n            {\n              \"description\": \"The issuer certificate identifier.\"\n            }\n          ]\n        },\n        \"deviceCertificateArn\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/CertificateArn\"\n            },\n            {\n              \"description\": \"The ARN of the identified device certificate.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Information that identifies the noncompliant resource.\"\n    },\n    \"expirationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n     \
  \   {\n          \"description\": \" The epoch timestamp in seconds at which this suppression expires. \"\n        }\n      ]\n    },\n    \"suppressIndefinitely\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SuppressIndefinitely\"\n        },\n        {\n          \"description\": \" Indicates whether a suppression should exist indefinitely or not. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditDescription\"\n        },\n        {\n          \"description\": \" The description of the audit suppression. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-audit-suppression-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeAuditSuppressionResponse
---
