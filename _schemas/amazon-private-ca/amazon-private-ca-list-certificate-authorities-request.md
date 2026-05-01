---
description: ListCertificateAuthoritiesRequest schema from Amazon Private CA API
layout: schema
name: ListCertificateAuthoritiesRequest
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: ResourceOwner
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-list-certificate-authorities-request-schema.json
slug: amazon-private-ca-list-certificate-authorities-request
source_filename: amazon-private-ca-list-certificate-authorities-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-list-certificate-authorities-request-schema.json\",\n  \"title\": \"ListCertificateAuthoritiesRequest\",\n  \"description\": \"ListCertificateAuthoritiesRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"Use this parameter when paginating results in a subsequent request after you receive a response with truncated results. Set it to the value of the <code>NextToken</code> parameter from the response you just received.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n    \
  \      \"description\": \"Use this parameter when paginating results to specify the maximum number of items to return in the response on each page. If additional items exist beyond the number you specify, the <code>NextToken</code> element is sent in the response. Use this <code>NextToken</code> value in a subsequent request to retrieve additional items.\"\n        }\n      ]\n    },\n    \"ResourceOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceOwner\"\n        },\n        {\n          \"description\": \"Use this parameter to filter the returned set of certificate authorities based on their owner. The default is SELF.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-list-certificate-authorities-request-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: ListCertificateAuthoritiesRequest
---
