---
description: The result returned by the Apidog API after an export operation, containing the exported API specification data.
layout: schema
name: Apidog Export Result
properties_list:
- description: Whether the export operation completed successfully.
  name: success
  type: boolean
- description: The exported API specification data as a string in the requested format (JSON or YAML).
  name: data
  type: string
provider_name: Apidog
provider_slug: apidog
schema_file: json-schema/apidog-export-result-schema.json
slug: apidog-export-result
tags:
- API Design
- API Lifecycle
- API Testing
- Collaboration
- Design-First
- Documentation
- Mocking
- Platform
title: Apidog Export Result
---
