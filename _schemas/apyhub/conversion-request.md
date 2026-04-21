---
description: A document or data conversion request to the ApyHub API
layout: schema
name: ConversionRequest
properties_list:
- description: Unique conversion request identifier
  name: requestId
  type: string
- description: Conversion operation type
  name: type
  type: string
- description: URL of the input file to convert
  name: inputUrl
  type: string
- description: Desired output format
  name: outputFormat
  type: string
- description: Conversion status
  name: status
  type: string
- description: URL of the converted output file
  name: outputUrl
  type: string
- description: Request creation timestamp
  name: createdAt
  type: string
provider_name: ApyHub
provider_slug: apyhub
schema_file: json-schema/conversion-request-schema.json
slug: conversion-request
tags:
- API Platform
- Data Processing
- Document Conversion
- Utility APIs
title: ConversionRequest
---
