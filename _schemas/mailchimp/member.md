---
description: A member (subscriber/contact) of a Mailchimp audience/list. Represents an individual who is currently or has been previously subscribed to a list, including members who have bounced or unsubscribed.
layout: schema
name: Mailchimp List Member
properties_list:
- description: The MD5 hash of the lowercase version of the list member's email address. This serves as the unique identifier for a member within a list.
  name: id
  type: string
- description: Email address for the subscriber.
  name: email_address
  type: string
- description: An identifier for the address across all of Mailchimp.
  name: unique_email_id
  type: string
- description: A contact identifier that is agnostic of email address. As Mailchimp evolves beyond email, contacts may exist without an email address.
  name: contact_id
  type: string
- description: The contact's full name.
  name: full_name
  type: string
- description: The ID used in the Mailchimp web application.
  name: web_id
  type: integer
- description: Type of email this member asked to get ('html' or 'text').
  name: email_type
  type: string
- description: Subscriber's current status.
  name: status
  type: string
- description: A subscriber's reason for unsubscribing.
  name: unsubscribe_reason
  type: string
- description: Indicates whether a contact consents to 1:1 messaging.
  name: consents_to_one_to_one_messaging
  type: boolean
- description: A US phone number for SMS contact.
  name: sms_phone_number
  type: string
- description: The status of an SMS subscription.
  name: sms_subscription_status
  type: string
- description: The datetime when the SMS subscription was last updated.
  name: sms_subscription_last_updated
  type: string
- description: A dictionary of merge fields where the keys are the merge tags (e.g., FNAME, LNAME). Values are the corresponding merge field values.
  name: merge_fields
  type: object
- description: The key of this object's properties is the ID of the interest in question, and the value is a boolean indicating whether the member is in that interest group.
  name: interests
  type: object
- description: Open and click rates for this subscriber.
  name: stats
  type: object
- description: IP address the subscriber signed up from.
  name: ip_signup
  type: string
- description: The date and time the subscriber signed up for the list in ISO 8601 format.
  name: timestamp_signup
  type: string
- description: The IP address the subscriber used to confirm their opt-in status.
  name: ip_opt
  type: string
- description: The date and time the subscriber confirmed their opt-in status in ISO 8601 format.
  name: timestamp_opt
  type: string
- description: Star rating for this member, between 1 and 5.
  name: member_rating
  type: integer
- description: The date and time the member's info was last changed in ISO 8601 format.
  name: last_changed
  type: string
- description: If set/detected, the subscriber's language.
  name: language
  type: string
- description: VIP status for subscriber.
  name: vip
  type: boolean
- description: The list member's email client.
  name: email_client
  type: string
- description: Subscriber location information.
  name: location
  type: object
- description: The marketing permissions for the subscriber.
  name: marketing_permissions
  type: array
- description: The most recent note added about this member.
  name: last_note
  type: object
- description: The source from which the subscriber was added to this list.
  name: source
  type: string
- description: The number of tags applied to this member.
  name: tags_count
  type: integer
- description: Tags applied to the member for additional segmentation and organization.
  name: tags
  type: array
- description: The list ID that this member belongs to.
  name: list_id
  type: string
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/member.json
slug: member
source_filename: member.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/messaging/mailchimp/json-schema/member.json\",\n  \"title\": \"Mailchimp List Member\",\n  \"description\": \"A member (subscriber/contact) of a Mailchimp audience/list. Represents an individual who is currently or has been previously subscribed to a list, including members who have bounced or unsubscribed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The MD5 hash of the lowercase version of the list member's email address. This serves as the unique identifier for a member within a list.\",\n      \"readOnly\": true\n    },\n    \"email_address\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address for the subscriber.\"\n    },\n    \"unique_email_id\": {\n      \"type\": \"string\",\n      \"description\": \"An identifier for the address across\
  \ all of Mailchimp.\",\n      \"readOnly\": true\n    },\n    \"contact_id\": {\n      \"type\": \"string\",\n      \"description\": \"A contact identifier that is agnostic of email address. As Mailchimp evolves beyond email, contacts may exist without an email address.\",\n      \"readOnly\": true\n    },\n    \"full_name\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's full name.\",\n      \"readOnly\": true\n    },\n    \"web_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID used in the Mailchimp web application.\",\n      \"readOnly\": true\n    },\n    \"email_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of email this member asked to get ('html' or 'text').\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Subscriber's current status.\",\n      \"enum\": [\"subscribed\", \"unsubscribed\", \"cleaned\", \"pending\", \"transactional\", \"archived\"]\n    },\n    \"unsubscribe_reason\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"A subscriber's reason for unsubscribing.\"\n    },\n    \"consents_to_one_to_one_messaging\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether a contact consents to 1:1 messaging.\",\n      \"readOnly\": true\n    },\n    \"sms_phone_number\": {\n      \"type\": \"string\",\n      \"description\": \"A US phone number for SMS contact.\"\n    },\n    \"sms_subscription_status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of an SMS subscription.\",\n      \"enum\": [\"subscribed\", \"unsubscribed\", \"nonsubscribed\", \"pending\"]\n    },\n    \"sms_subscription_last_updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The datetime when the SMS subscription was last updated.\"\n    },\n    \"merge_fields\": {\n      \"type\": \"object\",\n      \"description\": \"A dictionary of merge fields where the keys are the merge tags (e.g.,\
  \ FNAME, LNAME). Values are the corresponding merge field values.\",\n      \"additionalProperties\": true\n    },\n    \"interests\": {\n      \"type\": \"object\",\n      \"description\": \"The key of this object's properties is the ID of the interest in question, and the value is a boolean indicating whether the member is in that interest group.\",\n      \"additionalProperties\": {\n        \"type\": \"boolean\"\n      }\n    },\n    \"stats\": {\n      \"type\": \"object\",\n      \"description\": \"Open and click rates for this subscriber.\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"avg_open_rate\": {\n          \"type\": \"number\",\n          \"description\": \"A subscriber's average open rate.\",\n          \"readOnly\": true\n        },\n        \"avg_click_rate\": {\n          \"type\": \"number\",\n          \"description\": \"A subscriber's average clickthrough rate.\",\n          \"readOnly\": true\n        },\n        \"ecommerce_data\": {\n       \
  \   \"type\": \"object\",\n          \"description\": \"Ecommerce stats for the list member if the list is attached to a store.\",\n          \"readOnly\": true,\n          \"properties\": {\n            \"total_revenue\": {\n              \"type\": \"number\",\n              \"description\": \"The total revenue the list member has brought in.\"\n            },\n            \"number_of_orders\": {\n              \"type\": \"number\",\n              \"description\": \"The total number of orders placed by the list member.\"\n            },\n            \"currency_code\": {\n              \"type\": \"string\",\n              \"description\": \"The three-letter ISO 4217 code for the currency that the store accepts.\"\n            }\n          }\n        }\n      }\n    },\n    \"ip_signup\": {\n      \"type\": \"string\",\n      \"description\": \"IP address the subscriber signed up from.\",\n      \"readOnly\": true\n    },\n    \"timestamp_signup\": {\n      \"type\": \"string\",\n     \
  \ \"format\": \"date-time\",\n      \"description\": \"The date and time the subscriber signed up for the list in ISO 8601 format.\",\n      \"readOnly\": true\n    },\n    \"ip_opt\": {\n      \"type\": \"string\",\n      \"description\": \"The IP address the subscriber used to confirm their opt-in status.\",\n      \"readOnly\": true\n    },\n    \"timestamp_opt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the subscriber confirmed their opt-in status in ISO 8601 format.\",\n      \"readOnly\": true\n    },\n    \"member_rating\": {\n      \"type\": \"integer\",\n      \"description\": \"Star rating for this member, between 1 and 5.\",\n      \"minimum\": 1,\n      \"maximum\": 5,\n      \"readOnly\": true\n    },\n    \"last_changed\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the member's info was last changed in ISO 8601 format.\",\n      \"readOnly\"\
  : true\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"If set/detected, the subscriber's language.\"\n    },\n    \"vip\": {\n      \"type\": \"boolean\",\n      \"description\": \"VIP status for subscriber.\"\n    },\n    \"email_client\": {\n      \"type\": \"string\",\n      \"description\": \"The list member's email client.\",\n      \"readOnly\": true\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"description\": \"Subscriber location information.\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\",\n          \"description\": \"The location latitude.\"\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"description\": \"The location longitude.\"\n        },\n        \"gmtoff\": {\n          \"type\": \"integer\",\n          \"description\": \"The time difference in hours from GMT.\",\n          \"readOnly\": true\n        },\n        \"dstoff\": {\n          \"\
  type\": \"integer\",\n          \"description\": \"The offset for timezones where daylight saving time is observed.\",\n          \"readOnly\": true\n        },\n        \"country_code\": {\n          \"type\": \"string\",\n          \"description\": \"The unique code for the location country.\",\n          \"readOnly\": true\n        },\n        \"timezone\": {\n          \"type\": \"string\",\n          \"description\": \"The timezone for the location.\",\n          \"readOnly\": true\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"The region for the location.\",\n          \"readOnly\": true\n        }\n      }\n    },\n    \"marketing_permissions\": {\n      \"type\": \"array\",\n      \"description\": \"The marketing permissions for the subscriber.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"marketing_permission_id\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"The ID for the marketing permission.\"\n          },\n          \"text\": {\n            \"type\": \"string\",\n            \"description\": \"The text of the marketing permission.\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the subscriber has opted in to this permission.\"\n          }\n        }\n      }\n    },\n    \"last_note\": {\n      \"type\": \"object\",\n      \"description\": \"The most recent note added about this member.\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"note_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The note ID.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the note was created in ISO 8601 format.\"\n        },\n        \"created_by\": {\n          \"type\": \"string\",\n          \"description\": \"The author of the note.\"\
  \n        },\n        \"note\": {\n          \"type\": \"string\",\n          \"description\": \"The content of the note.\"\n        }\n      }\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The source from which the subscriber was added to this list.\",\n      \"readOnly\": true\n    },\n    \"tags_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of tags applied to this member.\",\n      \"readOnly\": true\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags applied to the member for additional segmentation and organization.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"The tag ID.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The tag name.\"\n          }\n        }\n      },\n      \"readOnly\": true\n    },\n\
  \    \"list_id\": {\n      \"type\": \"string\",\n      \"description\": \"The list ID that this member belongs to.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"email_address\", \"status\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/member.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: Mailchimp List Member
---
