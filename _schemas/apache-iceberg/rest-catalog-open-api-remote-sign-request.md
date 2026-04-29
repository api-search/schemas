---
description: The request to be signed remotely.
layout: schema
name: RemoteSignRequest
properties_list:
- description: ''
  name: region
  type: string
- description: ''
  name: uri
  type: string
- description: ''
  name: method
  type: string
- description: ''
  name: headers
  type: object
- description: ''
  name: properties
  type: object
- description: Optional body of the request to send to the signing API. This should only be populated for requests where the body of the message contains content which must be validated before a request is signed, s
  name: body
  type: string
- description: 'The storage provider for which the request is to be signed. The provider should correspond to the scheme used for a storage native URI. For example `s3` for AWS S3 paths. For backwards compatibility, '
  name: provider
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-remote-sign-request-schema.json
slug: rest-catalog-open-api-remote-sign-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remote-sign-request-schema.json\",\n  \"title\": \"RemoteSignRequest\",\n  \"description\": \"The request to be signed remotely.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"region\": {\n      \"type\": \"string\"\n    },\n    \"uri\": {\n      \"type\": \"string\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PUT\",\n        \"GET\",\n        \"HEAD\",\n        \"POST\",\n        \"DELETE\",\n        \"PATCH\",\n        \"OPTIONS\"\n      ]\n    },\n    \"headers\": {\n      \"$ref\": \"#/components/schemas/MultiValuedMap\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Optional body of the request to send to the signing API. This should only be populated for requests where the body of the message contains content which must be validated before a request is signed, such as the S3 DeleteObjects call.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The storage provider for which the request is to be signed. The provider should correspond to the scheme used for a storage native URI. For example `s3` for AWS S3 paths. For backwards compatibility, if this is not specified, the provider is assumed to be `s3`.\"\n    }\n  },\n  \"required\": [\n    \"region\",\n    \"uri\",\n    \"method\",\n    \"headers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remote-sign-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: RemoteSignRequest
---
