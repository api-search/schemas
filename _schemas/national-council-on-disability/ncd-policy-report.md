---
description: A policy report published by the National Council on Disability containing recommendations to the President, Congress, or federal agencies.
layout: schema
name: NCD Policy Report
properties_list:
- description: Full title of the NCD policy report
  name: title
  type: string
- description: Date the report was published
  name: publicationDate
  type: string
- description: Primary policy area covered by the report
  name: policyArea
  type: string
- description: Executive summary or abstract of the report
  name: summary
  type: string
- description: List of policy recommendations made in the report
  name: recommendations
  type: array
- description: URL to download the full report
  name: documentURL
  type: string
- description: Document file format
  name: format
  type: string
- description: Publication year
  name: year
  type: integer
provider_name: National Council on Disability
provider_slug: national-council-on-disability
schema_file: json-schema/ncd-policy-report-schema.json
slug: ncd-policy-report
tags:
- Disability
- Federal Government
- Policy
- Civil Rights
- Healthcare
- Independent Agency
title: NCD Policy Report
---
