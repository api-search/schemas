---
description: Contains information about the client certificate authentication settings for the <code>RegisterCertificate</code> and <code>DescribeCertificate</code> operations.
layout: schema
name: ClientCertAuthSettings
properties_list:
- description: ''
  name: OCSPUrl
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-client-cert-auth-settings-schema.json
slug: amazon-directory-service-client-cert-auth-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-client-cert-auth-settings-schema.json\",\n  \"title\": \"ClientCertAuthSettings\",\n  \"description\": \"Contains information about the client certificate authentication settings for the <code>RegisterCertificate</code> and <code>DescribeCertificate</code> operations. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OCSPUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OCSPUrl\"\n        },\n        {\n          \"description\": \"Specifies the URL of the default OCSP server used to check for revocation status. A secondary value to any OCSP address found in the AIA extension of the user certificate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-client-cert-auth-settings-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: ClientCertAuthSettings
---
