---
description: Represents a CMS delivery channel used for publishing and delivering managed content to Experience Cloud sites or external applications.
layout: schema
name: CMS Channel
properties_list:
- description: Unique identifier of the CMS channel
  name: channelId
  type: string
- description: Display name of the channel
  name: channelName
  type: string
- description: Type of the delivery channel
  name: channelType
  type: string
- description: Domain associated with the channel for content delivery
  name: domain
  type: string
- description: Fully qualified domain name of the channel
  name: domainName
  type: string
- description: Whether the domain is locked and cannot be changed
  name: isDomainLocked
  type: boolean
- description: Whether content in this channel is searchable by site visitors
  name: isSearchable
  type: boolean
provider_name: Salesforce Experience Cloud
provider_slug: salesforce-experience-cloud
schema_file: json-schema/salesforce-experience-cloud-cms-channel-schema.json
slug: salesforce-experience-cloud-cms-channel
source_filename: salesforce-experience-cloud-cms-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/experience-cloud/cms-channel.json\",\n  \"title\": \"CMS Channel\",\n  \"description\": \"Represents a CMS delivery channel used for publishing and delivering managed content to Experience Cloud sites or external applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channelId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the CMS channel\"\n    },\n    \"channelName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the channel\"\n    },\n    \"channelType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the delivery channel\",\n      \"enum\": [\"ExperienceCloudSite\", \"CustomChannel\"]\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Domain associated with the channel for content delivery\"\n    },\n    \"domainName\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"Fully qualified domain name of the channel\"\n    },\n    \"isDomainLocked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain is locked and cannot be changed\",\n      \"default\": false\n    },\n    \"isSearchable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether content in this channel is searchable by site visitors\",\n      \"default\": true\n    }\n  },\n  \"required\": [\"channelId\", \"channelName\", \"channelType\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/json-schema/salesforce-experience-cloud-cms-channel-schema.json
tags:
- CMS
- Communities
- CRM
- Customer Portal
- Digital Experience
- Experience Cloud
- Partner Portal
title: CMS Channel
---
