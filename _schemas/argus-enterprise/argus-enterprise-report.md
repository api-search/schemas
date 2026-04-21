---
description: Report schema from ARGUS Enterprise API
layout: schema
name: Report
properties_list:
- description: Unique report identifier
  name: id
  type: string
- description: Type of report
  name: reportType
  type: string
- description: Report title
  name: title
  type: string
- description: Report generation status
  name: status
  type: string
- description: Report generation timestamp
  name: generatedAt
  type: string
- description: URL to download the completed report
  name: downloadUrl
  type: string
- description: Parameters used to generate the report
  name: parameters
  type: object
- description: Username of the report creator
  name: createdBy
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-report-schema.json
slug: argus-enterprise-report
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Report
---
