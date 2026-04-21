---
description: Properties to attach new disk to the Virtual Machine.
layout: schema
name: AttachNewDataDiskOptions
properties_list:
- description: The name of the disk to be attached.
  name: diskName
  type: string
- description: Size of the disk to be attached in GibiBytes.
  name: diskSizeGiB
  type: integer
- description: The storage type for the disk (i.e. Standard, Premium).
  name: diskType
  type: string
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-attach-new-data-disk-options-schema.json
slug: azure-test-labs-attach-new-data-disk-options
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: AttachNewDataDiskOptions
---
