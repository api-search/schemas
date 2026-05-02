---
description: A Lyft ride representing a transportation request from an origin to a destination, including status, driver, vehicle, and pricing information.
layout: schema
name: Lyft Ride
properties_list:
- description: Unique identifier for the ride.
  name: ride_id
  type: string
- description: Identifier for the type of Lyft ride.
  name: ride_type
  type: string
- description: Current status of the ride.
  name: status
  type: string
- description: Pickup location for the ride.
  name: origin
  type: object
- description: Drop-off location for the ride.
  name: destination
  type: object
- description: Actual pickup location recorded by the driver.
  name: pickup
  type: object
- description: Actual drop-off location recorded by the driver.
  name: dropoff
  type: object
- description: Information about the driver assigned to this ride.
  name: driver
  type: object
- description: Information about the vehicle assigned to this ride.
  name: vehicle
  type: object
- description: Contact information for the ride passenger, used in concierge rides.
  name: passenger
  type: object
- description: Timestamp when the ride was requested.
  name: requested_at
  type: string
- description: Timestamp when the ride was completed.
  name: completed_at
  type: string
- description: Timestamp when the ride was canceled, if applicable.
  name: canceled_at
  type: string
- description: Scheduled pickup time for rides booked in advance.
  name: scheduled_pickup_time
  type: string
- description: Price information for the ride.
  name: price
  type: object
- description: Prime Time pricing percentage applied to this ride.
  name: primetime_percentage
  type: string
provider_name: lyft
provider_slug: lyft
schema_file: json-schema/lyft-ride-schema.json
slug: lyft-ride
source_filename: lyft-ride-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://lyft.com/schemas/lyft/ride.json\",\n  \"title\": \"Lyft Ride\",\n  \"description\": \"A Lyft ride representing a transportation request from an origin to a destination, including status, driver, vehicle, and pricing information.\",\n  \"type\": \"object\",\n  \"required\": [\"ride_id\", \"ride_type\", \"status\", \"origin\"],\n  \"properties\": {\n    \"ride_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the ride.\"\n    },\n    \"ride_type\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the type of Lyft ride.\",\n      \"enum\": [\"lyft\", \"lyft_line\", \"lyft_plus\", \"lyft_premier\", \"lyft_lux\", \"lyft_luxsuv\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the ride.\",\n      \"enum\": [\"pending\", \"accepted\", \"arrived\", \"pickedUp\", \"droppedOff\", \"canceled\"\
  , \"unknown\"]\n    },\n    \"origin\": {\n      \"$ref\": \"#/$defs/Location\",\n      \"description\": \"Pickup location for the ride.\"\n    },\n    \"destination\": {\n      \"$ref\": \"#/$defs/Location\",\n      \"description\": \"Drop-off location for the ride.\"\n    },\n    \"pickup\": {\n      \"$ref\": \"#/$defs/Location\",\n      \"description\": \"Actual pickup location recorded by the driver.\"\n    },\n    \"dropoff\": {\n      \"$ref\": \"#/$defs/Location\",\n      \"description\": \"Actual drop-off location recorded by the driver.\"\n    },\n    \"driver\": {\n      \"$ref\": \"#/$defs/Driver\",\n      \"description\": \"Information about the driver assigned to this ride.\"\n    },\n    \"vehicle\": {\n      \"$ref\": \"#/$defs/Vehicle\",\n      \"description\": \"Information about the vehicle assigned to this ride.\"\n    },\n    \"passenger\": {\n      \"$ref\": \"#/$defs/Passenger\",\n      \"description\": \"Contact information for the ride passenger, used in concierge\
  \ rides.\"\n    },\n    \"requested_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the ride was requested.\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the ride was completed.\"\n    },\n    \"canceled_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the ride was canceled, if applicable.\"\n    },\n    \"scheduled_pickup_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled pickup time for rides booked in advance.\"\n    },\n    \"price\": {\n      \"$ref\": \"#/$defs/Price\",\n      \"description\": \"Price information for the ride.\"\n    },\n    \"primetime_percentage\": {\n      \"type\": \"string\",\n      \"description\": \"Prime Time pricing percentage applied to this ride.\"\n    }\n  },\n  \"$defs\": {\n\
  \    \"Location\": {\n      \"type\": \"object\",\n      \"description\": \"A geographic location with coordinates and optional address information.\",\n      \"required\": [\"lat\", \"lng\"],\n      \"properties\": {\n        \"lat\": {\n          \"type\": \"number\",\n          \"description\": \"Latitude of the location.\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"lng\": {\n          \"type\": \"number\",\n          \"description\": \"Longitude of the location.\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Street address of the location.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City name.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"State or province code.\"\n        },\n        \"zip\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"Postal code.\"\n        }\n      }\n    },\n    \"Driver\": {\n      \"type\": \"object\",\n      \"description\": \"Information about a Lyft driver.\",\n      \"properties\": {\n        \"first_name\": {\n          \"type\": \"string\",\n          \"description\": \"The driver's first name.\"\n        },\n        \"phone_number\": {\n          \"type\": \"string\",\n          \"description\": \"The driver's contact phone number.\"\n        },\n        \"rating\": {\n          \"type\": \"string\",\n          \"description\": \"The driver's average rating.\"\n        },\n        \"image_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the driver's profile photo.\"\n        }\n      }\n    },\n    \"Vehicle\": {\n      \"type\": \"object\",\n      \"description\": \"Information about a vehicle used for a Lyft ride.\",\n      \"properties\": {\n        \"make\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"Vehicle manufacturer name.\"\n        },\n        \"model\": {\n          \"type\": \"string\",\n          \"description\": \"Vehicle model name.\"\n        },\n        \"year\": {\n          \"type\": \"integer\",\n          \"description\": \"Vehicle model year.\",\n          \"minimum\": 1900,\n          \"maximum\": 2100\n        },\n        \"license_plate\": {\n          \"type\": \"string\",\n          \"description\": \"Vehicle license plate number.\"\n        },\n        \"license_plate_state\": {\n          \"type\": \"string\",\n          \"description\": \"State where the vehicle is registered.\",\n          \"minLength\": 2,\n          \"maxLength\": 2\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"Color of the vehicle.\"\n        },\n        \"image_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to an image of the vehicle.\"\n      \
  \  }\n      }\n    },\n    \"Passenger\": {\n      \"type\": \"object\",\n      \"description\": \"Contact information for a ride passenger.\",\n      \"required\": [\"first_name\", \"phone_number\"],\n      \"properties\": {\n        \"first_name\": {\n          \"type\": \"string\",\n          \"description\": \"First name of the passenger.\"\n        },\n        \"last_name\": {\n          \"type\": \"string\",\n          \"description\": \"Last name of the passenger.\"\n        },\n        \"phone_number\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number where the passenger can be reached.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address for the passenger.\"\n        }\n      }\n    },\n    \"Price\": {\n      \"type\": \"object\",\n      \"description\": \"Price information for a ride.\",\n      \"properties\": {\n        \"amount\": {\n          \"type\"\
  : \"integer\",\n          \"description\": \"Total price in the smallest denomination of the currency.\",\n          \"minimum\": 0\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 4217 currency code.\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the price.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/json-schema/lyft-ride-schema.json
tags: []
title: Lyft Ride
---
