---
description: Represents an in-flight deployment package associated with an Appian application. Contains metadata about the package contents and status.
layout: schema
name: Package
properties_list:
- description: The name of the deployment package.
  name: name
  type: string
- description: A description of the deployment package.
  name: description
  type: string
- description: The unique identifier for the package. This UUID can be used with the Deployment REST API for exports and deployments.
  name: uuid
  type: string
- description: The number of design objects included in the package.
  name: objectCount
  type: integer
- description: The number of database scripts included in the package.
  name: databaseScriptCount
  type: integer
- description: The number of plug-ins included in the package.
  name: pluginCount
  type: integer
- description: The UUID of the data source associated with the package, if applicable.
  name: datasourceUuid
  type: string
- description: Indicates whether the package includes an import customization file.
  name: hasCustomizationFile
  type: boolean
- description: The timestamp when the package was created.
  name: createdTimestamp
  type: string
- description: The timestamp when the package was last modified. Packages are sorted by this field in descending order.
  name: lastModifiedTimestamp
  type: string
- description: A link to an external ticket or change request associated with this package.
  name: ticketLink
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/application-package-details-package-schema.json
slug: application-package-details-package
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: Package
---
