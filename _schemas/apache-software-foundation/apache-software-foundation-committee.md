---
description: Schema for an Apache Software Foundation Project Management Committee (PMC) as returned by the Projects and Whimsy APIs.
layout: schema
name: Apache Software Foundation Committee
properties_list:
- description: The committee display name
  name: name
  type: string
- description: Apache ID of the committee chair
  name: chair
  type: string
- description: A brief description of the committee
  name: description
  type: string
- description: The committee homepage URL
  name: homepage
  type: string
- description: Date the committee was established (e.g., 2002-01)
  name: established
  type: string
- description: Whether this is a Project Management Committee
  name: pmc
  type: boolean
- description: Reporting schedule months (e.g., ['January', 'April', 'July', 'October'])
  name: report
  type: array
- description: Committee roster keyed by Apache ID
  name: roster
  type: object
- description: Number of members in the committee roster
  name: roster_count
  type: integer
provider_name: Apache Software Foundation
provider_slug: apache-software-foundation
schema_file: json-schema/apache-software-foundation-committee-schema.json
slug: apache-software-foundation-committee
tags:
- ASF
- Open Source
- Governance
- Projects
- Apache
title: Apache Software Foundation Committee
---
