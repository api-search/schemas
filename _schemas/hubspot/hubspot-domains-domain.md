---
description: Represents a domain connected to a HubSpot CMS site
layout: schema
name: Domain
properties_list:
- description: The unique identifier for the domain
  name: id
  type: string
- description: The actual domain or sub-domain (e.g., www.hubspot.com)
  name: domain
  type: string
- description: When the domain was created
  name: createdAt
  type: string
- description: When the domain was last updated
  name: updatedAt
  type: string
- description: Whether the DNS for this domain is optimally configured for use with HubSpot
  name: isResolving
  type: boolean
- description: Whether the domain has been manually marked as resolving
  name: isManuallyMarkedAsResolving
  type: boolean
- description: Whether SSL is enabled for this domain
  name: isSslEnabled
  type: boolean
- description: Whether the domain only accepts HTTPS connections
  name: isSslOnly
  type: boolean
- description: Whether this is the primary domain for blog posts
  name: isPrimaryBlogPost
  type: boolean
- description: Whether this is the primary domain for site pages
  name: isPrimarySitePage
  type: boolean
- description: Whether this is the primary domain for landing pages
  name: isPrimaryLandingPage
  type: boolean
- description: Whether this is the primary domain for email web pages
  name: isPrimaryEmail
  type: boolean
- description: Whether this is the primary domain for knowledge base
  name: isPrimaryKnowledge
  type: boolean
- description: Whether the domain is used for CMS blog posts
  name: isUsedForBlogPost
  type: boolean
- description: Whether the domain is used for CMS site pages
  name: isUsedForSitePage
  type: boolean
- description: Whether the domain is used for CMS landing pages
  name: isUsedForLandingPage
  type: boolean
- description: Whether the domain is used for CMS email web pages
  name: isUsedForEmail
  type: boolean
- description: Whether the domain is used for CMS knowledge pages
  name: isUsedForKnowledge
  type: boolean
- description: The expected CNAME record for this domain
  name: expectedCname
  type: string
- description: The domain to redirect to, if any
  name: redirectTo
  type: string
- description: The primary domain this domain is secondary to
  name: secondaryToDomain
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-domains-domain-schema.json
slug: hubspot-domains-domain
source_filename: hubspot-domains-domain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents a domain connected to a HubSpot CMS site\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the domain\",\n      \"example\": \"3210329704\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The actual domain or sub-domain (e.g., www.hubspot.com)\",\n      \"example\": \"99558489.hubspot.com\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the domain was created\",\n      \"format\": \"date-time\",\n      \"example\": \"2017-07-11T13:00:52.928Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the domain was last updated\",\n      \"format\": \"date-time\",\n      \"example\": \"2019-10-08T16:54:57.165Z\"\n    },\n    \"isResolving\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DNS for this domain is optimally\
  \ configured for use with HubSpot\",\n      \"example\": true\n    },\n    \"isManuallyMarkedAsResolving\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain has been manually marked as resolving\",\n      \"example\": false\n    },\n    \"isSslEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether SSL is enabled for this domain\",\n      \"example\": true\n    },\n    \"isSslOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain only accepts HTTPS connections\",\n      \"example\": false\n    },\n    \"isPrimaryBlogPost\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the primary domain for blog posts\",\n      \"example\": true\n    },\n    \"isPrimarySitePage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the primary domain for site pages\",\n      \"example\": false\n    },\n    \"isPrimaryLandingPage\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether this is the primary domain for landing pages\",\n      \"example\": false\n    },\n    \"isPrimaryEmail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the primary domain for email web pages\",\n      \"example\": false\n    },\n    \"isPrimaryKnowledge\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the primary domain for knowledge base\",\n      \"example\": false\n    },\n    \"isUsedForBlogPost\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain is used for CMS blog posts\",\n      \"example\": true\n    },\n    \"isUsedForSitePage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain is used for CMS site pages\",\n      \"example\": false\n    },\n    \"isUsedForLandingPage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain is used for CMS landing pages\",\n      \"example\": false\n    },\n    \"isUsedForEmail\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Whether the domain is used for CMS email web pages\",\n      \"example\": false\n    },\n    \"isUsedForKnowledge\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain is used for CMS knowledge pages\",\n      \"example\": false\n    },\n    \"expectedCname\": {\n      \"type\": \"string\",\n      \"description\": \"The expected CNAME record for this domain\",\n      \"example\": \"99558489.group39.sites.hubspot.net\"\n    },\n    \"redirectTo\": {\n      \"type\": \"string\",\n      \"description\": \"The domain to redirect to, if any\",\n      \"example\": \"\"\n    },\n    \"secondaryToDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The primary domain this domain is secondary to\",\n      \"example\": \"example.hubspot.com\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"domain\",\n    \"isResolving\",\n    \"isUsedForBlogPost\",\n    \"isUsedForSitePage\",\n    \"isUsedForLandingPage\",\n   \
  \ \"isUsedForEmail\",\n    \"isUsedForKnowledge\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Domain\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-domains-domain-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: Domain
---
