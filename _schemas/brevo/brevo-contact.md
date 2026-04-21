---
description: Represents a contact in the Brevo platform with email, phone, attributes, and list memberships used for transactional and marketing messaging.
layout: schema
name: Brevo Contact
properties_list:
- description: Unique internal identifier of the contact.
  name: id
  type: integer
- description: Primary email address of the contact.
  name: email
  type: string
- description: Phone number of the contact in international format.
  name: phone
  type: string
- description: Whether the contact's email address is blacklisted from receiving messages.
  name: emailBlacklisted
  type: boolean
- description: Whether the contact's phone number is blacklisted from receiving SMS.
  name: smsBlacklisted
  type: boolean
- description: IDs of contact lists the contact belongs to.
  name: listIds
  type: array
- description: Custom attribute values for the contact profile as key-value pairs. Keys correspond to attribute names defined in the account.
  name: attributes
  type: object
- description: UTC date-time when the contact was created.
  name: createdAt
  type: string
- description: UTC date-time when the contact was last modified.
  name: modifiedAt
  type: string
- description: Email campaign interaction statistics for the contact.
  name: statistics
  type: object
provider_name: brevo
provider_slug: brevo
schema_file: json-schema/brevo-contact-schema.json
slug: brevo-contact
tags: []
title: Brevo Contact
---
