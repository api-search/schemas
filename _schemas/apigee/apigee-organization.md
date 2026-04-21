---
description: Represents an Apigee organization, the top-level container for all Apigee resources including API proxies, products, developers, and environments.
layout: schema
name: Apigee Organization
properties_list:
- description: Output only. Name of the Apigee organization.
  name: name
  type: string
- description: Display name for the organization.
  name: displayName
  type: string
- description: Description of the organization.
  name: description
  type: string
- description: Output only. Project ID associated with the organization.
  name: projectId
  type: string
- description: Output only. Time the organization was created in milliseconds since epoch.
  name: createdAt
  type: string
- description: Output only. Time the organization was last modified in milliseconds since epoch.
  name: lastModifiedAt
  type: string
- description: Output only. Subscription type of the organization.
  name: subscriptionType
  type: string
- description: Output only. State of the organization.
  name: state
  type: string
- description: Required. Primary Google Cloud region for analytics data storage.
  name: analyticsRegion
  type: string
- description: Required. Runtime type of the Apigee organization.
  name: runtimeType
  type: string
- description: VPC network used for service networking.
  name: authorizedNetwork
  type: string
- description: Output only. List of environments in the organization.
  name: environments
  type: array
- description: Billing type of the organization.
  name: billingType
  type: string
- description: A collection of key-value property pairs.
  name: properties
  type: object
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-organization-schema.json
slug: apigee-organization
tags:
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Hybrid
- Integrations
- Microservices
- Monetization
title: Apigee Organization
---
