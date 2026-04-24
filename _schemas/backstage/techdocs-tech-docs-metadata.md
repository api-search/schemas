---
description: TechDocsMetadata schema from Backstage techdocs API
layout: schema
name: TechDocsMetadata
properties_list:
- description: The name of the documentation site.
  name: site_name
  type: string
- description: Description of the documentation site.
  name: site_description
  type: string
- description: ETag for cache validation.
  name: etag
  type: string
- description: Timestamp of the last documentation build.
  name: build_timestamp
  type: string
- description: List of files in the documentation bundle.
  name: files
  type: array
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/techdocs-tech-docs-metadata-schema.json
slug: techdocs-tech-docs-metadata
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: TechDocsMetadata
---
