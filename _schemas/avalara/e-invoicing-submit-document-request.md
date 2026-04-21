---
description: SubmitDocumentRequest schema from Avalara API
layout: schema
name: SubmitDocumentRequest
properties_list:
- description: Format of the e-invoice document
  name: dataFormat
  type: string
- description: Version of the data format
  name: dataFormatVersion
  type: string
- description: Base64-encoded document content or raw UBL/CII XML
  name: data
  type: string
- description: ''
  name: metadata
  type: object
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-submit-document-request-schema.json
slug: e-invoicing-submit-document-request
tags:
- Taxes
title: SubmitDocumentRequest
---
