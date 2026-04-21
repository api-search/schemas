---
description: Schema for an Apache Software Foundation Incubator podling as returned by the Projects and Whimsy APIs.
layout: schema
name: Apache Software Foundation Podling
properties_list:
- description: The podling display name
  name: name
  type: string
- description: Current incubation status of the podling
  name: status
  type: string
- description: A brief description of the podling
  name: description
  type: string
- description: The podling homepage URL
  name: homepage
  type: string
- description: Date the podling entered incubation
  name: startdate
  type: string
- description: Date the podling left incubation (graduated or retired)
  name: enddate
  type: string
- description: The sponsoring PMC or Incubator
  name: sponsor
  type: string
- description: Apache ID of the podling champion
  name: champion
  type: string
- description: List of mentor Apache IDs
  name: mentors
  type: array
- description: Resolution details if the podling graduated or retired
  name: resolution
  type: string
provider_name: Apache Software Foundation
provider_slug: apache-software-foundation
schema_file: json-schema/apache-software-foundation-podling-schema.json
slug: apache-software-foundation-podling
tags:
- ASF
- Open Source
- Governance
- Projects
- Apache
title: Apache Software Foundation Podling
---
