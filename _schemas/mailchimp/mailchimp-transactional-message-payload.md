---
description: The message object containing all parameters for a transactional email, including recipients, content, attachments, and tracking options.
layout: schema
name: MessagePayload
properties_list:
- description: The full HTML content of the message.
  name: html
  type: string
- description: The full plain-text content of the message.
  name: text
  type: string
- description: The message subject line.
  name: subject
  type: string
- description: The sender email address.
  name: from_email
  type: string
- description: The sender display name.
  name: from_name
  type: string
- description: An array of recipient objects.
  name: to
  type: array
- description: Optional extra headers to add to the message (e.g., Reply-To).
  name: headers
  type: object
- description: Whether this message is important and should be delivered ahead of non-important messages.
  name: important
  type: boolean
- description: Whether to enable open tracking for this message.
  name: track_opens
  type: boolean
- description: Whether to enable click tracking for this message.
  name: track_clicks
  type: boolean
- description: Whether to automatically generate a plain-text version from the HTML content.
  name: auto_text
  type: boolean
- description: Whether to automatically generate HTML from the plain-text content.
  name: auto_html
  type: boolean
- description: Whether to automatically inline all CSS styles from style blocks in the HTML content.
  name: inline_css
  type: boolean
- description: Whether to strip query strings from URLs when aggregating tracked click data.
  name: url_strip_qs
  type: boolean
- description: Whether to show all recipients in the To header of each email.
  name: preserve_recipients
  type: boolean
- description: Whether to include a View Content Link in the Mandrill dashboard for this message.
  name: view_content_link
  type: boolean
- description: An optional address to BCC on the message.
  name: bcc_address
  type: string
- description: A custom domain to use for tracking opens and clicks.
  name: tracking_domain
  type: string
- description: A custom domain to use for DKIM signing instead of the default.
  name: signing_domain
  type: string
- description: A custom domain to use for the return-path header.
  name: return_path_domain
  type: string
- description: Whether to evaluate merge tags in the message.
  name: merge
  type: boolean
- description: The merge tag language to use (Mailchimp or Handlebars).
  name: merge_language
  type: string
- description: Global merge variables applied to all recipients.
  name: global_merge_vars
  type: array
- description: Per-recipient merge variables.
  name: merge_vars
  type: array
- description: An array of string tags to apply to this message for analytics.
  name: tags
  type: array
- description: The unique ID of a subaccount for this message.
  name: subaccount
  type: string
- description: An array of domains for which Google Analytics tracking parameters will be appended.
  name: google_analytics_domains
  type: array
- description: The utm_campaign tracking parameter for Google Analytics.
  name: google_analytics_campaign
  type: string
- description: Key-value metadata to associate with the message.
  name: metadata
  type: object
- description: Per-recipient metadata.
  name: recipient_metadata
  type: array
- description: An array of file attachments.
  name: attachments
  type: array
- description: An array of inline images referenced with "cid:" in the HTML content.
  name: images
  type: array
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-message-payload-schema.json
slug: mailchimp-transactional-message-payload
source_filename: mailchimp-transactional-message-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessagePayload\",\n  \"type\": \"object\",\n  \"description\": \"The message object containing all parameters for a transactional email, including recipients, content, attachments, and tracking options.\",\n  \"properties\": {\n    \"html\": {\n      \"type\": \"string\",\n      \"description\": \"The full HTML content of the message.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The full plain-text content of the message.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The message subject line.\"\n    },\n    \"from_email\": {\n      \"type\": \"string\",\n      \"description\": \"The sender email address.\"\n    },\n    \"from_name\": {\n      \"type\": \"string\",\n      \"description\": \"The sender display name.\"\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"description\": \"An array of recipient objects.\"\
  \n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Optional extra headers to add to the message (e.g., Reply-To).\"\n    },\n    \"important\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this message is important and should be delivered ahead of non-important messages.\"\n    },\n    \"track_opens\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable open tracking for this message.\"\n    },\n    \"track_clicks\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable click tracking for this message.\"\n    },\n    \"auto_text\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to automatically generate a plain-text version from the HTML content.\"\n    },\n    \"auto_html\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to automatically generate HTML from the plain-text content.\"\n    },\n    \"inline_css\": {\n      \"type\": \"boolean\",\n     \
  \ \"description\": \"Whether to automatically inline all CSS styles from style blocks in the HTML content.\"\n    },\n    \"url_strip_qs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to strip query strings from URLs when aggregating tracked click data.\"\n    },\n    \"preserve_recipients\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to show all recipients in the To header of each email.\"\n    },\n    \"view_content_link\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include a View Content Link in the Mandrill dashboard for this message.\"\n    },\n    \"bcc_address\": {\n      \"type\": \"string\",\n      \"description\": \"An optional address to BCC on the message.\"\n    },\n    \"tracking_domain\": {\n      \"type\": \"string\",\n      \"description\": \"A custom domain to use for tracking opens and clicks.\"\n    },\n    \"signing_domain\": {\n      \"type\": \"string\",\n      \"description\": \"A custom domain\
  \ to use for DKIM signing instead of the default.\"\n    },\n    \"return_path_domain\": {\n      \"type\": \"string\",\n      \"description\": \"A custom domain to use for the return-path header.\"\n    },\n    \"merge\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to evaluate merge tags in the message.\"\n    },\n    \"merge_language\": {\n      \"type\": \"string\",\n      \"description\": \"The merge tag language to use (Mailchimp or Handlebars).\"\n    },\n    \"global_merge_vars\": {\n      \"type\": \"array\",\n      \"description\": \"Global merge variables applied to all recipients.\"\n    },\n    \"merge_vars\": {\n      \"type\": \"array\",\n      \"description\": \"Per-recipient merge variables.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"An array of string tags to apply to this message for analytics.\"\n    },\n    \"subaccount\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of a subaccount\
  \ for this message.\"\n    },\n    \"google_analytics_domains\": {\n      \"type\": \"array\",\n      \"description\": \"An array of domains for which Google Analytics tracking parameters will be appended.\"\n    },\n    \"google_analytics_campaign\": {\n      \"type\": \"string\",\n      \"description\": \"The utm_campaign tracking parameter for Google Analytics.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value metadata to associate with the message.\"\n    },\n    \"recipient_metadata\": {\n      \"type\": \"array\",\n      \"description\": \"Per-recipient metadata.\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"An array of file attachments.\"\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"description\": \"An array of inline images referenced with \\\"cid:\\\" in the HTML content.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-message-payload-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: MessagePayload
---
