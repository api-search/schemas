---
description: An event happening at a certain time and location, such as a concert, lecture, or festival.
layout: schema
name: Schema.org Event
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: The JSON-LD context URL.
  name: '@context'
  type: string
- description: The name of the event.
  name: name
  type: string
- description: A description of the event.
  name: description
  type: string
- description: URL of the event.
  name: url
  type: string
- description: An image of the event.
  name: image
  type: object
- description: The start date and time of the event.
  name: startDate
  type: string
- description: The end date and time of the event.
  name: endDate
  type: string
- description: The time admission will commence.
  name: doorTime
  type: string
- description: The duration of the event in ISO 8601 format.
  name: duration
  type: string
- description: The status of the event.
  name: eventStatus
  type: string
- description: The attendance mode of the event.
  name: eventAttendanceMode
  type: string
- description: The location of the event.
  name: location
  type: object
- description: An organizer of an Event.
  name: organizer
  type: object
- description: A performer at the event.
  name: performer
  type: object
- description: A person or organization that supports a thing through a pledge, promise, or financial contribution.
  name: sponsor
  type: object
- description: An offer to provide this item.
  name: offers
  type: object
- description: An intended audience.
  name: audience
  type: object
- description: The total number of individuals that may attend.
  name: maximumAttendeeCapacity
  type: integer
- description: The maximum virtual attendee capacity.
  name: maximumVirtualAttendeeCapacity
  type: integer
- description: The number of attendee places remaining.
  name: remainingAttendeeCapacity
  type: integer
- description: Used for rescheduled or cancelled events to indicate the original start date.
  name: previousStartDate
  type: string
- description: An event that this event is a part of.
  name: superEvent
  type: object
- description: An Event that is part of this event.
  name: subEvent
  type: object
- description: The language of the event.
  name: inLanguage
  type: string
- description: A flag to signal that the item is accessible for free.
  name: isAccessibleForFree
  type: boolean
- description: A review of the event.
  name: review
  type: object
- description: The overall rating, based on a collection of reviews or ratings.
  name: aggregateRating
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
- description: The identifier property represents any kind of identifier.
  name: identifier
  type: string
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-event-schema.json
slug: schema-org-event
source_filename: schema-org-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/event.json\",\n  \"title\": \"Schema.org Event\",\n  \"description\": \"An event happening at a certain time and location, such as a concert, lecture, or festival.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"Event\", \"BusinessEvent\", \"ChildrensEvent\", \"ComedyEvent\", \"CourseInstance\", \"DanceEvent\", \"DeliveryEvent\", \"EducationEvent\", \"ExhibitionEvent\", \"Festival\", \"FoodEvent\", \"Hackathon\", \"LiteraryEvent\", \"MusicEvent\", \"PublicationEvent\", \"SaleEvent\", \"ScreeningEvent\", \"SocialEvent\", \"SportsEvent\", \"TheaterEvent\", \"VisualArtsEvent\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"description\": \"The JSON-LD context URL.\",\n      \"default\": \"https://schema.org\"\
  \n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the event.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the event.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the event.\"\n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An image of the event.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The start date and time of the event.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The end date and time of the event.\"\n    },\n    \"doorTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"The time admission will commence.\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"The duration of the event in ISO 8601 format.\"\n    },\n    \"eventStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"EventCancelled\", \"EventMovedOnline\", \"EventPostponed\", \"EventRescheduled\", \"EventScheduled\"],\n      \"description\": \"The status of the event.\"\n    },\n    \"eventAttendanceMode\": {\n      \"type\": \"string\",\n      \"enum\": [\"MixedEventAttendanceMode\", \"OfflineEventAttendanceMode\", \"OnlineEventAttendanceMode\"],\n      \"description\": \"The attendance mode of the event.\"\n    },\n    \"location\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"$ref\": \"schema-org-place-schema.json\" },\n        { \"$ref\": \"#/$defs/VirtualLocation\" },\n        { \"$ref\": \"schema-org-postal-address-schema.json\" }\n      ],\n      \"description\": \"The location of the event.\"\n    },\n    \"organizer\"\
  : {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"An organizer of an Event.\"\n    },\n    \"performer\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"oneOf\": [{ \"$ref\": \"schema-org-person-schema.json\" }, { \"$ref\": \"schema-org-organization-schema.json\" }] } }\n      ],\n      \"description\": \"A performer at the event.\"\n    },\n    \"sponsor\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"A person or organization that supports a thing through a pledge, promise, or financial contribution.\"\n    },\n    \"offers\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-offer-schema.json\"\
  \ },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-offer-schema.json\" } }\n      ],\n      \"description\": \"An offer to provide this item.\"\n    },\n    \"audience\": {\n      \"type\": \"object\",\n      \"description\": \"An intended audience.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"Audience\" },\n        \"audienceType\": { \"type\": \"string\", \"description\": \"The target group.\" }\n      }\n    },\n    \"maximumAttendeeCapacity\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of individuals that may attend.\"\n    },\n    \"maximumVirtualAttendeeCapacity\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum virtual attendee capacity.\"\n    },\n    \"remainingAttendeeCapacity\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of attendee places remaining.\"\n    },\n    \"previousStartDate\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"Used for rescheduled or cancelled events to indicate the original start date.\"\n    },\n    \"superEvent\": {\n      \"$ref\": \"#\",\n      \"description\": \"An event that this event is a part of.\"\n    },\n    \"subEvent\": {\n      \"oneOf\": [\n        { \"$ref\": \"#\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#\" } }\n      ],\n      \"description\": \"An Event that is part of this event.\"\n    },\n    \"inLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"The language of the event.\"\n    },\n    \"isAccessibleForFree\": {\n      \"type\": \"boolean\",\n      \"description\": \"A flag to signal that the item is accessible for free.\"\n    },\n    \"review\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-review-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-review-schema.json\" } }\n      ],\n      \"description\": \"A review of the event.\"\n    },\n\
  \    \"aggregateRating\": {\n      \"$ref\": \"schema-org-aggregate-rating-schema.json\",\n      \"description\": \"The overall rating, based on a collection of reviews or ratings.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier property represents any kind of identifier.\"\n    }\n  },\n  \"$defs\": {\n    \"VirtualLocation\": {\n      \"type\": \"object\",\n      \"description\": \"An online or virtual location for attending events.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"VirtualLocation\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"URL of the\
  \ virtual location.\" },\n        \"name\": { \"type\": \"string\", \"description\": \"Name of the virtual location or platform.\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-event-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org Event
---
