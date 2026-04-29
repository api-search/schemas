---
description: Permissions designate which private CA actions can be performed by an Amazon Web Services service or entity. In order for ACM to automatically renew private certificates, you must give the ACM service principal all available permissions (<code>IssueCertificate</code>, <code>GetCertificate</code>, and <code>ListPermissions</code>). Permissions can be assigned with the <a href="https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreatePermission.html">CreatePermission</a> action, removed with the <a href="https://docs.aws.amazon.com/privateca/latest/APIReference/API_DeletePermission.html">DeletePermission</a> action, and listed with the <a href="https://docs.aws.amazon.com/privateca/latest/APIReference/API_ListPermissions.html">ListPermissions</a> action.
layout: schema
name: Permission
properties_list:
- description: ''
  name: CertificateAuthorityArn
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: Principal
  type: object
- description: ''
  name: SourceAccount
  type: object
- description: ''
  name: Actions
  type: object
- description: ''
  name: Policy
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-permission-schema.json
slug: amazon-private-ca-permission
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-permission-schema.json\",\n  \"title\": \"Permission\",\n  \"description\": \"Permissions designate which private CA actions can be performed by an Amazon Web Services service or entity. In order for ACM to automatically renew private certificates, you must give the ACM service principal all available permissions (<code>IssueCertificate</code>, <code>GetCertificate</code>, and <code>ListPermissions</code>). Permissions can be assigned with the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreatePermission.html\\\">CreatePermission</a> action, removed with the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_DeletePermission.html\\\">DeletePermission</a> action, and listed with the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_ListPermissions.html\\\
  \">ListPermissions</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the private CA from which the permission was issued.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The time at which the permission was created.\"\n        }\n      ]\n    },\n    \"Principal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Principal\"\n        },\n        {\n          \"description\": \"The Amazon Web Services service or entity that holds the permission. At this time, the only valid principal is <code>acm.amazonaws.com</code>.\"\n        }\n      ]\n    },\n    \"SourceAccount\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the account that assigned the permission.\"\n        }\n      ]\n    },\n    \"Actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionList\"\n        },\n        {\n          \"description\": \"The private CA actions that can be performed by the designated Amazon Web Services service.\"\n        }\n      ]\n    },\n    \"Policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AWSPolicy\"\n        },\n        {\n          \"description\": \"The name of the policy that is associated with the permission.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-permission-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: Permission
---
