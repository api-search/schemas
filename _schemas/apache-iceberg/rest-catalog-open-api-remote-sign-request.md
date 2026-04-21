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
