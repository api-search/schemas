---
description: A place as represented by the Google Maps Places API (New). Contains comprehensive information about a physical location including identity, contact details, location data, ratings, reviews, opening hours, and service options. Based on the Google Maps Platform Places API documentation.
layout: schema
name: Google Maps Place
properties_list:
- description: The resource name of this place in the format places/{placeId}
  name: name
  type: string
- description: The unique place ID. A textual identifier that uniquely identifies a place in the Google Places database and on Google Maps.
  name: id
  type: string
- description: The localized display name of the place, suitable for short textual identification
  name: displayName
  type: object
- description: A set of type tags for this place. A place can have multiple types. Full list defined by Google Maps Place Types.
  name: types
  type: array
- description: The primary type of this place, representing the most specific type tag
  name: primaryType
  type: string
- description: The display name of the primary type, localized to the request language
  name: primaryTypeDisplayName
  type: object
- description: The place's phone number in national format
  name: nationalPhoneNumber
  type: string
- description: The place's phone number in international format, including country code
  name: internationalPhoneNumber
  type: string
- description: The full human-readable address for this place, including street, city, state/province, postal code, and country
  name: formattedAddress
  type: string
- description: A short human-readable address, typically including only the street address and city
  name: shortFormattedAddress
  type: string
- description: The individual address components of the place's address, broken down by type (street number, route, locality, etc.)
  name: addressComponents
  type: array
- description: The geographic location of the place as latitude/longitude coordinates
  name: location
  type: object
- description: A viewport suitable for displaying the place on a map of average size
  name: viewport
  type: object
- description: The place's overall rating based on aggregated user reviews, on a scale of 1.0 to 5.0
  name: rating
  type: number
- description: The total number of user ratings that contributed to the place's overall rating
  name: userRatingCount
  type: integer
- description: A URL pointing to this place's page on Google Maps
  name: googleMapsUri
  type: string
- description: The authoritative website URL for this place, if known
  name: websiteUri
  type: string
- description: The regular (non-holiday) opening hours for this place
  name: regularOpeningHours
  type: object
- description: The current opening hours, which may differ from regular hours due to holidays or special events
  name: currentOpeningHours
  type: object
- description: The price level of the place, indicating relative cost
  name: priceLevel
  type: string
- description: The operational status of the business
  name: businessStatus
  type: string
- description: Number of minutes this place's current timezone is offset from UTC
  name: utcOffsetMinutes
  type: integer
- description: A list of up to 5 reviews for this place, sorted by relevance
  name: reviews
  type: array
- description: Photos associated with this place, including references for fetching photo media
  name: photos
  type: array
- description: A brief editorial summary of the place, written by Google
  name: editorialSummary
  type: object
- description: The place's address in adr microformat (http://microformats.org/wiki/adr)
  name: adrFormatAddress
  type: string
- description: A URL to an SVG icon mask that can be used to represent the place's type
  name: iconMaskBaseUri
  type: string
- description: The background color for the place's type icon, in hex format
  name: iconBackgroundColor
  type: string
- description: The Open Location Code (plus code) for this place
  name: plusCode
  type: object
- description: Accessibility features available at this place
  name: accessibilityOptions
  type: object
- description: Parking options available at this place
  name: parkingOptions
  type: object
- description: Payment methods accepted at this place
  name: paymentOptions
  type: object
- description: Whether the place supports dine-in service
  name: dineIn
  type: boolean
- description: Whether the place offers takeout service
  name: takeout
  type: boolean
- description: Whether the place offers delivery service
  name: delivery
  type: boolean
- description: Whether the place offers curbside pickup
  name: curbsidePickup
  type: boolean
- description: Whether the place accepts reservations
  name: reservable
  type: boolean
- description: Whether the place serves breakfast
  name: servesBreakfast
  type: boolean
- description: Whether the place serves lunch
  name: servesLunch
  type: boolean
- description: Whether the place serves dinner
  name: servesDinner
  type: boolean
- description: Whether the place serves beer
  name: servesBeer
  type: boolean
- description: Whether the place serves wine
  name: servesWine
  type: boolean
- description: Whether the place serves vegetarian food
  name: servesVegetarianFood
  type: boolean
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-place-schema.json
slug: google-maps-place
source_filename: google-maps-place-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/google-maps/json-schema/google-maps-place-schema.json\",\n  \"title\": \"Google Maps Place\",\n  \"description\": \"A place as represented by the Google Maps Places API (New). Contains comprehensive information about a physical location including identity, contact details, location data, ratings, reviews, opening hours, and service options. Based on the Google Maps Platform Places API documentation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of this place in the format places/{placeId}\",\n      \"pattern\": \"^places/.+$\",\n      \"examples\": [\"places/ChIJN1t_tDeuEmsRUsoyG83frY4\"]\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique place ID. A textual identifier that uniquely identifies a place in the Google Places database\
  \ and on Google Maps.\",\n      \"examples\": [\"ChIJN1t_tDeuEmsRUsoyG83frY4\"]\n    },\n    \"displayName\": {\n      \"$ref\": \"#/$defs/LocalizedText\",\n      \"description\": \"The localized display name of the place, suitable for short textual identification\"\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"A set of type tags for this place. A place can have multiple types. Full list defined by Google Maps Place Types.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [[\"restaurant\", \"food\", \"point_of_interest\", \"establishment\"]]\n    },\n    \"primaryType\": {\n      \"type\": \"string\",\n      \"description\": \"The primary type of this place, representing the most specific type tag\",\n      \"examples\": [\"restaurant\", \"cafe\", \"park\", \"museum\"]\n    },\n    \"primaryTypeDisplayName\": {\n      \"$ref\": \"#/$defs/LocalizedText\",\n      \"description\": \"The display name of the primary type, localized\
  \ to the request language\"\n    },\n    \"nationalPhoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The place's phone number in national format\",\n      \"examples\": [\"(02) 9374 4000\"]\n    },\n    \"internationalPhoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The place's phone number in international format, including country code\",\n      \"examples\": [\"+61 2 9374 4000\"]\n    },\n    \"formattedAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The full human-readable address for this place, including street, city, state/province, postal code, and country\",\n      \"examples\": [\"48 Pirrama Rd, Pyrmont NSW 2009, Australia\"]\n    },\n    \"shortFormattedAddress\": {\n      \"type\": \"string\",\n      \"description\": \"A short human-readable address, typically including only the street address and city\",\n      \"examples\": [\"48 Pirrama Rd, Pyrmont\"]\n    },\n    \"addressComponents\": {\n      \"type\": \"\
  array\",\n      \"description\": \"The individual address components of the place's address, broken down by type (street number, route, locality, etc.)\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AddressComponent\"\n      }\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/LatLng\",\n      \"description\": \"The geographic location of the place as latitude/longitude coordinates\"\n    },\n    \"viewport\": {\n      \"$ref\": \"#/$defs/Viewport\",\n      \"description\": \"A viewport suitable for displaying the place on a map of average size\"\n    },\n    \"rating\": {\n      \"type\": \"number\",\n      \"description\": \"The place's overall rating based on aggregated user reviews, on a scale of 1.0 to 5.0\",\n      \"minimum\": 1.0,\n      \"maximum\": 5.0,\n      \"examples\": [4.2]\n    },\n    \"userRatingCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of user ratings that contributed to the place's overall rating\",\n      \"minimum\"\
  : 0,\n      \"examples\": [1234]\n    },\n    \"googleMapsUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL pointing to this place's page on Google Maps\"\n    },\n    \"websiteUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The authoritative website URL for this place, if known\"\n    },\n    \"regularOpeningHours\": {\n      \"$ref\": \"#/$defs/OpeningHours\",\n      \"description\": \"The regular (non-holiday) opening hours for this place\"\n    },\n    \"currentOpeningHours\": {\n      \"$ref\": \"#/$defs/OpeningHours\",\n      \"description\": \"The current opening hours, which may differ from regular hours due to holidays or special events\"\n    },\n    \"priceLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The price level of the place, indicating relative cost\",\n      \"enum\": [\n        \"PRICE_LEVEL_UNSPECIFIED\",\n        \"PRICE_LEVEL_FREE\",\n        \"PRICE_LEVEL_INEXPENSIVE\"\
  ,\n        \"PRICE_LEVEL_MODERATE\",\n        \"PRICE_LEVEL_EXPENSIVE\",\n        \"PRICE_LEVEL_VERY_EXPENSIVE\"\n      ]\n    },\n    \"businessStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The operational status of the business\",\n      \"enum\": [\n        \"BUSINESS_STATUS_UNSPECIFIED\",\n        \"OPERATIONAL\",\n        \"CLOSED_TEMPORARILY\",\n        \"CLOSED_PERMANENTLY\"\n      ]\n    },\n    \"utcOffsetMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of minutes this place's current timezone is offset from UTC\"\n    },\n    \"reviews\": {\n      \"type\": \"array\",\n      \"description\": \"A list of up to 5 reviews for this place, sorted by relevance\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Review\"\n      },\n      \"maxItems\": 5\n    },\n    \"photos\": {\n      \"type\": \"array\",\n      \"description\": \"Photos associated with this place, including references for fetching photo media\",\n      \"items\": {\n\
  \        \"$ref\": \"#/$defs/Photo\"\n      }\n    },\n    \"editorialSummary\": {\n      \"$ref\": \"#/$defs/LocalizedText\",\n      \"description\": \"A brief editorial summary of the place, written by Google\"\n    },\n    \"adrFormatAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The place's address in adr microformat (http://microformats.org/wiki/adr)\"\n    },\n    \"iconMaskBaseUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL to an SVG icon mask that can be used to represent the place's type\"\n    },\n    \"iconBackgroundColor\": {\n      \"type\": \"string\",\n      \"description\": \"The background color for the place's type icon, in hex format\",\n      \"pattern\": \"^#[0-9A-Fa-f]{6}$\",\n      \"examples\": [\"#FF9E67\"]\n    },\n    \"plusCode\": {\n      \"$ref\": \"#/$defs/PlusCode\",\n      \"description\": \"The Open Location Code (plus code) for this place\"\n    },\n    \"accessibilityOptions\": {\n\
  \      \"$ref\": \"#/$defs/AccessibilityOptions\",\n      \"description\": \"Accessibility features available at this place\"\n    },\n    \"parkingOptions\": {\n      \"$ref\": \"#/$defs/ParkingOptions\",\n      \"description\": \"Parking options available at this place\"\n    },\n    \"paymentOptions\": {\n      \"$ref\": \"#/$defs/PaymentOptions\",\n      \"description\": \"Payment methods accepted at this place\"\n    },\n    \"dineIn\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place supports dine-in service\"\n    },\n    \"takeout\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place offers takeout service\"\n    },\n    \"delivery\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place offers delivery service\"\n    },\n    \"curbsidePickup\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place offers curbside pickup\"\n    },\n    \"reservable\": {\n      \"type\": \"boolean\",\n\
  \      \"description\": \"Whether the place accepts reservations\"\n    },\n    \"servesBreakfast\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place serves breakfast\"\n    },\n    \"servesLunch\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place serves lunch\"\n    },\n    \"servesDinner\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place serves dinner\"\n    },\n    \"servesBeer\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place serves beer\"\n    },\n    \"servesWine\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place serves wine\"\n    },\n    \"servesVegetarianFood\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place serves vegetarian food\"\n    }\n  },\n  \"required\": [\"name\", \"id\"],\n  \"$defs\": {\n    \"LocalizedText\": {\n      \"type\": \"object\",\n      \"description\": \"A localized text string with its associated\
  \ language code\",\n      \"properties\": {\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"The localized text value\"\n        },\n        \"languageCode\": {\n          \"type\": \"string\",\n          \"description\": \"The BCP-47 language code of the text\",\n          \"examples\": [\"en\", \"fr\", \"ja\"]\n        }\n      },\n      \"required\": [\"text\"]\n    },\n    \"LatLng\": {\n      \"type\": \"object\",\n      \"description\": \"A geographic coordinate expressed as latitude and longitude in decimal degrees (WGS84)\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\",\n          \"description\": \"Latitude in decimal degrees. Must be in the range [-90.0, +90.0].\",\n          \"minimum\": -90.0,\n          \"maximum\": 90.0,\n          \"examples\": [-33.8688]\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"description\": \"Longitude in decimal degrees. Must be in the range\
  \ [-180.0, +180.0].\",\n          \"minimum\": -180.0,\n          \"maximum\": 180.0,\n          \"examples\": [151.2093]\n        }\n      },\n      \"required\": [\"latitude\", \"longitude\"]\n    },\n    \"Viewport\": {\n      \"type\": \"object\",\n      \"description\": \"A rectangular viewport defined by its low (southwest) and high (northeast) points\",\n      \"properties\": {\n        \"low\": {\n          \"$ref\": \"#/$defs/LatLng\",\n          \"description\": \"The southwest corner of the viewport\"\n        },\n        \"high\": {\n          \"$ref\": \"#/$defs/LatLng\",\n          \"description\": \"The northeast corner of the viewport\"\n        }\n      },\n      \"required\": [\"low\", \"high\"]\n    },\n    \"AddressComponent\": {\n      \"type\": \"object\",\n      \"description\": \"An individual component of a structured address\",\n      \"properties\": {\n        \"longText\": {\n          \"type\": \"string\",\n          \"description\": \"The full text description\
  \ of the address component\",\n          \"examples\": [\"Mountain View\"]\n        },\n        \"shortText\": {\n          \"type\": \"string\",\n          \"description\": \"An abbreviated textual name for the address component\",\n          \"examples\": [\"MV\"]\n        },\n        \"types\": {\n          \"type\": \"array\",\n          \"description\": \"An array of strings indicating the type of this address component (e.g., locality, administrative_area_level_1, country)\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"languageCode\": {\n          \"type\": \"string\",\n          \"description\": \"The language code for this component\"\n        }\n      },\n      \"required\": [\"longText\", \"shortText\", \"types\"]\n    },\n    \"PlusCode\": {\n      \"type\": \"object\",\n      \"description\": \"An Open Location Code (plus code) representing a geographic area\",\n      \"properties\": {\n        \"globalCode\": {\n          \"\
  type\": \"string\",\n          \"description\": \"The full plus code (global code) that identifies a geographic area\",\n          \"examples\": [\"4RRH57G3+6R\"]\n        },\n        \"compoundCode\": {\n          \"type\": \"string\",\n          \"description\": \"The compound plus code, which includes a locality reference for easier human readability\",\n          \"examples\": [\"57G3+6R Pyrmont, New South Wales, Australia\"]\n        }\n      }\n    },\n    \"OpeningHours\": {\n      \"type\": \"object\",\n      \"description\": \"Information about when a place is open for business\",\n      \"properties\": {\n        \"openNow\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the place is currently open\"\n        },\n        \"periods\": {\n          \"type\": \"array\",\n          \"description\": \"Time periods the place is open during the week, structured as open/close pairs\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Period\"\n    \
  \      }\n        },\n        \"weekdayDescriptions\": {\n          \"type\": \"array\",\n          \"description\": \"Localized strings describing the opening hours for each day of the week\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"examples\": [[\"Monday: 9:00 AM - 5:00 PM\", \"Tuesday: 9:00 AM - 5:00 PM\"]]\n        }\n      }\n    },\n    \"Period\": {\n      \"type\": \"object\",\n      \"description\": \"A single time period when a place is open, defined by open and close points\",\n      \"properties\": {\n        \"open\": {\n          \"$ref\": \"#/$defs/TimePoint\",\n          \"description\": \"The time when the place opens\"\n        },\n        \"close\": {\n          \"$ref\": \"#/$defs/TimePoint\",\n          \"description\": \"The time when the place closes. Absent for places open 24 hours.\"\n        }\n      },\n      \"required\": [\"open\"]\n    },\n    \"TimePoint\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"A specific point in time on a weekly schedule\",\n      \"properties\": {\n        \"day\": {\n          \"type\": \"integer\",\n          \"description\": \"Day of the week as an integer (0 = Sunday, 6 = Saturday)\",\n          \"minimum\": 0,\n          \"maximum\": 6\n        },\n        \"hour\": {\n          \"type\": \"integer\",\n          \"description\": \"Hour in 24-hour format (0-23)\",\n          \"minimum\": 0,\n          \"maximum\": 23\n        },\n        \"minute\": {\n          \"type\": \"integer\",\n          \"description\": \"Minute of the hour (0-59)\",\n          \"minimum\": 0,\n          \"maximum\": 59\n        }\n      },\n      \"required\": [\"day\", \"hour\", \"minute\"]\n    },\n    \"Review\": {\n      \"type\": \"object\",\n      \"description\": \"A user-submitted review of a place\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The resource name of the review\"\n        },\n        \"\
  relativePublishTimeDescription\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable relative time description (e.g., 'a month ago')\",\n          \"examples\": [\"a month ago\", \"2 weeks ago\"]\n        },\n        \"rating\": {\n          \"type\": \"number\",\n          \"description\": \"The star rating of this review, from 1.0 to 5.0\",\n          \"minimum\": 1.0,\n          \"maximum\": 5.0\n        },\n        \"text\": {\n          \"$ref\": \"#/$defs/LocalizedText\",\n          \"description\": \"The review text\"\n        },\n        \"originalText\": {\n          \"$ref\": \"#/$defs/LocalizedText\",\n          \"description\": \"The review text in its original language\"\n        },\n        \"authorAttribution\": {\n          \"$ref\": \"#/$defs/AuthorAttribution\",\n          \"description\": \"Information about the review author\"\n        },\n        \"publishTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\
  ,\n          \"description\": \"The timestamp when the review was published\"\n        }\n      }\n    },\n    \"AuthorAttribution\": {\n      \"type\": \"object\",\n      \"description\": \"Attribution information for a content author\",\n      \"properties\": {\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the author\"\n        },\n        \"uri\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A URI to the author's profile\"\n        },\n        \"photoUri\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A URI to the author's profile photo\"\n        }\n      }\n    },\n    \"Photo\": {\n      \"type\": \"object\",\n      \"description\": \"A photo associated with a place\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The resource name of the photo in the\
  \ format places/{placeId}/photos/{photoReference}\",\n          \"pattern\": \"^places/.+/photos/.+$\"\n        },\n        \"widthPx\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum available width of the photo in pixels\",\n          \"minimum\": 1\n        },\n        \"heightPx\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum available height of the photo in pixels\",\n          \"minimum\": 1\n        },\n        \"authorAttributions\": {\n          \"type\": \"array\",\n          \"description\": \"The authors/contributors of this photo\",\n          \"items\": {\n            \"$ref\": \"#/$defs/AuthorAttribution\"\n          }\n        }\n      }\n    },\n    \"AccessibilityOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Accessibility features available at a place\",\n      \"properties\": {\n        \"wheelchairAccessibleParking\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether\
  \ the place has wheelchair-accessible parking\"\n        },\n        \"wheelchairAccessibleEntrance\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the place has a wheelchair-accessible entrance\"\n        },\n        \"wheelchairAccessibleRestroom\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the place has a wheelchair-accessible restroom\"\n        },\n        \"wheelchairAccessibleSeating\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the place has wheelchair-accessible seating\"\n        }\n      }\n    },\n    \"ParkingOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Parking options available at a place\",\n      \"properties\": {\n        \"freeParkingLot\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the place has a free parking lot\"\n        },\n        \"paidParkingLot\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether\
  \ the place has a paid parking lot\"\n        },\n        \"freeStreetParking\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether free street parking is available nearby\"\n        },\n        \"paidStreetParking\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether paid street parking is available nearby\"\n        },\n        \"valetParking\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the place offers valet parking\"\n        },\n        \"freeGarageParking\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the place has a free parking garage\"\n        },\n        \"paidGarageParking\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the place has a paid parking garage\"\n        }\n      }\n    },\n    \"PaymentOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Payment methods accepted at a place\",\n      \"properties\": {\n        \"\
  acceptsCreditCards\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the place accepts credit cards\"\n        },\n        \"acceptsDebitCards\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the place accepts debit cards\"\n        },\n        \"acceptsCashOnly\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the place only accepts cash\"\n        },\n        \"acceptsNfc\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the place accepts NFC/contactless payments\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-place-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: Google Maps Place
---
