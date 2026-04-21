---
description: Response containing the total count of packages and an array of package detail objects for the specified application.
layout: schema
name: PackageListResponse
properties_list:
- description: The total number of in-flight packages for the application. Maximum of 100.
  name: totalPackageCount
  type: integer
- description: Array of package objects ordered by last modified timestamp, newest first.
  name: packages
  type: array
provider_name: Appian
provider_slug: appian
schema_file: json-schema/application-package-details-package-list-response-schema.json
slug: application-package-details-package-list-response
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: PackageListResponse
---
