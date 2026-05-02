---
description: Schema for Litmus email test objects representing preview rendering, spam filter, and link-check test requests and results across email clients and filter services.
layout: schema
name: Litmus Email Test
properties_list:
- description: Unique numeric identifier for the email test
  name: id
  type: integer
- description: Overall processing status of the email test
  name: status
  type: string
- description: Email subject line submitted for testing
  name: subject
  type: string
- description: Sender email address used in spam filter evaluation
  name: from_address
  type: string
- description: Sender display name used in spam filter context
  name: from_name
  type: string
- description: Timestamp when the test was created
  name: created_at
  type: string
- description: Timestamp when all requested test types completed
  name: completed_at
  type: string
- description: Whether email client preview rendering was included in this test
  name: previews_requested
  type: boolean
- description: Whether spam filter testing was included in this test
  name: spam_requested
  type: boolean
- description: Whether link reachability checking was included in this test
  name: links_requested
  type: boolean
- description: Rendering results for each requested email client
  name: previews
  type: array
- description: Results from each spam filter service checked
  name: spam_results
  type: array
- description: Reachability results for each URL found in the email HTML
  name: link_results
  type: array
provider_name: Litmus
provider_slug: litmus
schema_file: json-schema/litmus-email-test-schema.json
slug: litmus-email-test
source_filename: litmus-email-test-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://litmus.com/schemas/litmus/email-test.json\",\n  \"title\": \"Litmus Email Test\",\n  \"description\": \"Schema for Litmus email test objects representing preview rendering, spam filter, and link-check test requests and results across email clients and filter services.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the email test\",\n      \"example\": 12345678\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Overall processing status of the email test\",\n      \"enum\": [\"pending\", \"processing\", \"complete\", \"failed\"]\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Email subject line submitted for testing\",\n      \"maxLength\": 998\n    },\n    \"from_address\": {\n   \
  \   \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Sender email address used in spam filter evaluation\"\n    },\n    \"from_name\": {\n      \"type\": \"string\",\n      \"description\": \"Sender display name used in spam filter context\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the test was created\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when all requested test types completed\"\n    },\n    \"previews_requested\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether email client preview rendering was included in this test\"\n    },\n    \"spam_requested\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether spam filter testing was included in this test\"\n    },\n    \"links_requested\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether link reachability checking was included in this test\"\n    },\n    \"previews\": {\n      \"type\": \"array\",\n      \"description\": \"Rendering results for each requested email client\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PreviewResult\"\n      }\n    },\n    \"spam_results\": {\n      \"type\": \"array\",\n      \"description\": \"Results from each spam filter service checked\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SpamResult\"\n      }\n    },\n    \"link_results\": {\n      \"type\": \"array\",\n      \"description\": \"Reachability results for each URL found in the email HTML\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LinkResult\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"PreviewResult\": {\n      \"type\": \"object\",\n      \"description\": \"Email rendering result for a single email client\",\n      \"required\": [\"client\", \"status\"],\n      \"properties\": {\n        \"client\": {\n          \"type\": \"string\",\n     \
  \     \"description\": \"Email client slug identifier\",\n          \"example\": \"GMAIL\"\n        },\n        \"client_name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable display name of the email client\",\n          \"example\": \"Gmail\"\n        },\n        \"platform\": {\n          \"type\": \"string\",\n          \"description\": \"Platform category of the email client\",\n          \"enum\": [\"desktop\", \"mobile\", \"webmail\"]\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Rendering completion status for this client\",\n          \"enum\": [\"pending\", \"processing\", \"complete\", \"failed\", \"unavailable\"]\n        },\n        \"full_image_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the full-size rendered screenshot image\"\n        },\n        \"thumb_image_url\": {\n          \"type\": \"string\",\n          \"format\"\
  : \"uri\",\n          \"description\": \"URL of the thumbnail rendered screenshot image\"\n        },\n        \"orientation\": {\n          \"type\": \"string\",\n          \"description\": \"Display orientation of the rendered screenshot\",\n          \"enum\": [\"desktop\", \"mobile\"]\n        }\n      }\n    },\n    \"SpamResult\": {\n      \"type\": \"object\",\n      \"description\": \"Result from a single spam filter service\",\n      \"required\": [\"filter\", \"status\"],\n      \"properties\": {\n        \"filter\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the spam filter service\",\n          \"example\": \"SpamAssassin\"\n        },\n        \"is_spam\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the email was flagged as spam by this filter\"\n        },\n        \"score\": {\n          \"type\": \"number\",\n          \"description\": \"Spam score returned by the filter (scale varies by provider)\"\n        },\n\
  \        \"threshold\": {\n          \"type\": \"number\",\n          \"description\": \"Spam score threshold above which the filter flags messages as spam\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Processing status of the spam filter check\",\n          \"enum\": [\"pending\", \"complete\", \"failed\"]\n        }\n      }\n    },\n    \"LinkResult\": {\n      \"type\": \"object\",\n      \"description\": \"Reachability check result for a single URL found in the email HTML\",\n      \"required\": [\"url\"],\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL that was checked for reachability\"\n        },\n        \"status_code\": {\n          \"type\": \"integer\",\n          \"description\": \"HTTP status code returned when the URL was fetched\",\n          \"minimum\": 100,\n          \"maximum\": 599\n        },\n        \"reachable\"\
  : {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the URL was successfully reachable at time of test\"\n        },\n        \"redirect_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Final destination URL after HTTP redirects, if applicable\"\n        }\n      }\n    },\n    \"EmailClient\": {\n      \"type\": \"object\",\n      \"description\": \"An email client available for preview rendering\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier or slug for the email client\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable display name of the email client\"\n        },\n        \"platform\": {\n          \"type\": \"string\",\n          \"description\": \"Platform category of the email client\",\n          \"enum\": [\"desktop\"\
  , \"mobile\", \"webmail\"]\n        },\n        \"available\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this client is currently available for rendering\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/json-schema/litmus-email-test-schema.json
tags:
- Developer Tools
- Email Testing
- Marketing Tools
- Quality Assurance
title: Litmus Email Test
---
