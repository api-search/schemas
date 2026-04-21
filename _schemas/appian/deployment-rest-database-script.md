---
description: Represents a database script included in an export or import deployment.
layout: schema
name: DatabaseScript
properties_list:
- description: The file name of the database script.
  name: fileName
  type: string
- description: The execution order of the database script, starting at 1.
  name: orderId
  type: integer
- description: URL to download the database script file.
  name: url
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-database-script-schema.json
slug: deployment-rest-database-script
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: DatabaseScript
---
