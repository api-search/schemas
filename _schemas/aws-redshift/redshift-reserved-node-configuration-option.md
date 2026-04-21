---
description: Details for a reserved-node exchange. Examples include the node type for a reserved node, the price for a node, the node's state, and other details.
layout: schema
name: ReservedNodeConfigurationOption
properties_list:
- description: Describes a reserved node. You can call the <a>DescribeReservedNodeOfferings</a> API to obtain the available reserved node offerings.
  name: SourceReservedNode
  type: object
- description: ''
  name: TargetReservedNodeCount
  type: object
- description: Describes a reserved node offering.
  name: TargetReservedNodeOffering
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-reserved-node-configuration-option-schema.json
slug: redshift-reserved-node-configuration-option
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ReservedNodeConfigurationOption
---
