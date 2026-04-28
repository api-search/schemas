---
description: Schema for a Cloud Custodian policy YAML file. A policy file contains one or more policies, each of which selects a cloud resource type, applies filters to narrow the set of matching resources, and executes actions against those resources. Policies can run in pull mode (on-demand), event mode (triggered by cloud events), periodic mode (scheduled), or config-rule mode (AWS Config). Cloud Custodian supports AWS, Azure, and GCP resource types.
layout: schema
name: Cloud Custodian Policy File
properties_list:
- description: List of one or more policy definitions in this file. Each policy selects a resource type and defines filters and actions to apply.
  name: policies
  type: array
- description: Global variable definitions that can be referenced across policies in this file using the {vars.varname} interpolation syntax.
  name: vars
  type: object
provider_name: Cloud Custodian
provider_slug: cloud-custodian
schema_file: json-schema/cloud-custodian-policy-schema.json
slug: cloud-custodian-policy
tags:
- Cloud Security
- Compliance
- Cost Optimization
- Multi-Cloud
- Policy as Code
title: Cloud Custodian Policy File
---
