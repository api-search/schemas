---
description: Properties of a schedules applicable to a virtual machine.
layout: schema
name: ApplicableSchedulePropertiesFragment
properties_list:
- description: The auto-shutdown schedule, if one has been set at the lab or lab resource level.
  name: labVmsShutdown
  type: object
- description: The auto-startup schedule, if one has been set at the lab or lab resource level.
  name: labVmsStartup
  type: object
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-applicable-schedule-properties-fragment-schema.json
slug: azure-test-labs-applicable-schedule-properties-fragment
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ApplicableSchedulePropertiesFragment
---
