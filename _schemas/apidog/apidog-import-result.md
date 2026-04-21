---
description: The result returned by the Apidog API after an import operation (OpenAPI, Swagger, or Postman Collection).
layout: schema
name: Apidog Import Result
properties_list:
- description: Whether the import operation completed successfully.
  name: success
  type: boolean
- description: Details about the imported resources.
  name: data
  type: object
provider_name: Apidog
provider_slug: apidog
schema_file: json-schema/apidog-import-result-schema.json
slug: apidog-import-result
tags:
- API Design
- API Lifecycle
- API Testing
- Collaboration
- Design-First
- Documentation
- Mocking
- Platform
title: Apidog Import Result
---
