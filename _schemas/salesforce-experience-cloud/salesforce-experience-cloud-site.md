---
description: Represents a Salesforce Experience Cloud site (community) with its configuration, status, and access settings.
layout: schema
name: Experience Cloud Site
properties_list:
- description: Unique 18-character Salesforce identifier for the site
  name: id
  type: string
- description: Display name of the Experience Cloud site
  name: name
  type: string
- description: Description of the site's purpose
  name: description
  type: string
- description: Current operational status of the site
  name: status
  type: string
- description: URL path prefix for the site, appended to the domain
  name: urlPathPrefix
  type: string
- description: Full URL of the Experience Cloud site
  name: siteUrl
  type: string
- description: URL for the site login page
  name: loginUrl
  type: string
- description: Name of the template used to create the site
  name: templateName
  type: string
- description: Whether guest users can access Chatter content without logging in
  name: allowChatterAccessWithoutLogin
  type: boolean
- description: Whether community members can flag content for moderation
  name: allowMembersToFlag
  type: boolean
- description: Whether site administrators can send invitations to join
  name: invitationsEnabled
  type: boolean
- description: Whether the knowledgeable people feature is enabled
  name: knowledgeableEnabled
  type: boolean
- description: Whether members can see other members in the site
  name: memberVisibilityEnabled
  type: boolean
- description: Whether nicknames are displayed instead of full names
  name: nicknameDisplayEnabled
  type: boolean
- description: Whether private messaging between members is enabled
  name: privateMessagesEnabled
  type: boolean
- description: Whether the reputation and points system is enabled
  name: reputationEnabled
  type: boolean
- description: Whether welcome emails are sent to new members
  name: sendWelcomeEmail
  type: boolean
- description: Whether the site-as-container feature is enabled for embedding
  name: siteAsContainerEnabled
  type: boolean
- description: API resource URL for this site
  name: url
  type: string
provider_name: Salesforce Experience Cloud
provider_slug: salesforce-experience-cloud
schema_file: json-schema/salesforce-experience-cloud-site-schema.json
slug: salesforce-experience-cloud-site
source_filename: salesforce-experience-cloud-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/experience-cloud/site.json\",\n  \"title\": \"Experience Cloud Site\",\n  \"description\": \"Represents a Salesforce Experience Cloud site (community) with its configuration, status, and access settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique 18-character Salesforce identifier for the site\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the Experience Cloud site\",\n      \"maxLength\": 80\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the site's purpose\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status of the site\",\n      \"enum\": [\"Live\", \"Inactive\", \"DownForMaintenance\", \"UnderConstruction\"\
  ]\n    },\n    \"urlPathPrefix\": {\n      \"type\": \"string\",\n      \"description\": \"URL path prefix for the site, appended to the domain\"\n    },\n    \"siteUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Full URL of the Experience Cloud site\"\n    },\n    \"loginUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for the site login page\"\n    },\n    \"templateName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the template used to create the site\"\n    },\n    \"allowChatterAccessWithoutLogin\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether guest users can access Chatter content without logging in\",\n      \"default\": false\n    },\n    \"allowMembersToFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether community members can flag content for moderation\",\n      \"default\": false\n    },\n    \"invitationsEnabled\": {\n \
  \     \"type\": \"boolean\",\n      \"description\": \"Whether site administrators can send invitations to join\",\n      \"default\": false\n    },\n    \"knowledgeableEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the knowledgeable people feature is enabled\",\n      \"default\": false\n    },\n    \"memberVisibilityEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether members can see other members in the site\",\n      \"default\": true\n    },\n    \"nicknameDisplayEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether nicknames are displayed instead of full names\",\n      \"default\": false\n    },\n    \"privateMessagesEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether private messaging between members is enabled\",\n      \"default\": false\n    },\n    \"reputationEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the reputation and points system is enabled\"\
  ,\n      \"default\": false\n    },\n    \"sendWelcomeEmail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether welcome emails are sent to new members\",\n      \"default\": true\n    },\n    \"siteAsContainerEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the site-as-container feature is enabled for embedding\",\n      \"default\": false\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API resource URL for this site\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/json-schema/salesforce-experience-cloud-site-schema.json
tags:
- CMS
- Communities
- CRM
- Customer Portal
- Digital Experience
- Experience Cloud
- Partner Portal
title: Experience Cloud Site
---
