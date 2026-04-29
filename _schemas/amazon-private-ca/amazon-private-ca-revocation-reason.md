---
description: RevocationReason schema from Amazon Private CA API
layout: schema
name: RevocationReason
properties_list: []
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-revocation-reason-schema.json
slug: amazon-private-ca-revocation-reason
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-revocation-reason-schema.json\",\n  \"title\": \"RevocationReason\",\n  \"description\": \"RevocationReason schema from Amazon Private CA API\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"UNSPECIFIED\",\n    \"KEY_COMPROMISE\",\n    \"CERTIFICATE_AUTHORITY_COMPROMISE\",\n    \"AFFILIATION_CHANGED\",\n    \"SUPERSEDED\",\n    \"CESSATION_OF_OPERATION\",\n    \"PRIVILEGE_WITHDRAWN\",\n    \"A_A_COMPROMISE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-revocation-reason-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: RevocationReason
---
