---
description: Schema for an Apache Software Foundation top-level project as returned by the Projects API.
layout: schema
name: Apache Software Foundation Project
properties_list:
- description: The official project name
  name: name
  type: string
- description: The project category (e.g., big-data, cloud, library)
  name: category
  type: string
- description: The Project Management Committee responsible for this project
  name: pmc
  type: string
- description: A brief description of the project
  name: description
  type: string
- description: The project homepage URL
  name: homepage
  type: string
- description: Primary programming language used by the project
  name: programming-language
  type: string
- description: URL of the project bug tracker
  name: bug-database
  type: string
- description: URL of the project downloads page
  name: download-page
  type: string
- description: URL of the project mailing list archives
  name: mailing-list
  type: string
- description: Source code repository URLs
  name: repository
  type: array
- description: The software license (typically Apache-2.0)
  name: license
  type: string
- description: A short one-line description of the project
  name: shortdesc
  type: string
provider_name: Apache Software Foundation
provider_slug: apache-software-foundation
schema_file: json-schema/apache-software-foundation-project-schema.json
slug: apache-software-foundation-project
tags:
- ASF
- Open Source
- Governance
- Projects
- Apache
title: Apache Software Foundation Project
---
