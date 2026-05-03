---
description: Represents a race or endurance event on the RunSignup platform. A race is the top-level container that holds one or more events (e.g., 5K, 10K, Half Marathon). The race object includes general information, location, registration settings, and links to events.
layout: schema
name: RunSignup Race
properties_list:
- description: Unique race identifier assigned by RunSignup.
  name: race_id
  type: integer
- description: The name of the race.
  name: name
  type: string
- description: The date of the next upcoming event in MM/DD/YYYY format.
  name: next_date
  type: string
- description: The end date of the next upcoming event in MM/DD/YYYY format.
  name: next_end_date
  type: string
- description: Whether this race is in draft mode (not published).
  name: is_draft_race
  type: string
- description: Whether this race is private (invitation only).
  name: is_private_race
  type: string
- description: Whether registration is currently open.
  name: is_registration_open
  type: string
- description: Date the race was created in the system.
  name: created
  type: string
- description: Date the race was last modified.
  name: last_modified
  type: string
- description: City where the race is held.
  name: city
  type: string
- description: US state abbreviation where the race is held.
  name: state
  type: string
- description: ISO country code for the race location.
  name: country_code
  type: string
- description: Postal code for the race location.
  name: zip
  type: string
- description: HTML or plain text description of the race.
  name: description
  type: string
- description: RunSignup registration page URL for the race.
  name: url
  type: string
- description: External race website URL provided by the race director.
  name: external_race_url
  type: string
- description: URL to the race logo image.
  name: logo_url
  type: string
- description: ID of the charity associated with this race for fundraising.
  name: charity_id
  type: integer
- description: List of events within this race (e.g., 5K, 10K, Half Marathon).
  name: events
  type: array
provider_name: RunSignup
provider_slug: runsignup
schema_file: json-schema/runsignup-race-schema.json
slug: runsignup-race
source_filename: runsignup-race-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://runsignup.com/schemas/runsignup/race.json\",\n  \"title\": \"RunSignup Race\",\n  \"description\": \"Represents a race or endurance event on the RunSignup platform. A race is the top-level container that holds one or more events (e.g., 5K, 10K, Half Marathon). The race object includes general information, location, registration settings, and links to events.\",\n  \"type\": \"object\",\n  \"required\": [\"race_id\", \"name\"],\n  \"properties\": {\n    \"race_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique race identifier assigned by RunSignup.\",\n      \"minimum\": 1\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the race.\",\n      \"minLength\": 1\n    },\n    \"next_date\": {\n      \"type\": \"string\",\n      \"description\": \"The date of the next upcoming event in MM/DD/YYYY format.\"\n    },\n    \"next_end_date\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The end date of the next upcoming event in MM/DD/YYYY format.\"\n    },\n    \"is_draft_race\": {\n      \"type\": \"string\",\n      \"description\": \"Whether this race is in draft mode (not published).\",\n      \"enum\": [\"T\", \"F\"]\n    },\n    \"is_private_race\": {\n      \"type\": \"string\",\n      \"description\": \"Whether this race is private (invitation only).\",\n      \"enum\": [\"T\", \"F\"]\n    },\n    \"is_registration_open\": {\n      \"type\": \"string\",\n      \"description\": \"Whether registration is currently open.\",\n      \"enum\": [\"T\", \"F\"]\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"Date the race was created in the system.\"\n    },\n    \"last_modified\": {\n      \"type\": \"string\",\n      \"description\": \"Date the race was last modified.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City where the race is held.\"\
  \n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"US state abbreviation where the race is held.\"\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO country code for the race location.\",\n      \"pattern\": \"^[A-Z]{2,3}$\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"Postal code for the race location.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"HTML or plain text description of the race.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"RunSignup registration page URL for the race.\"\n    },\n    \"external_race_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"External race website URL provided by the race director.\"\n    },\n    \"logo_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to\
  \ the race logo image.\"\n    },\n    \"charity_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the charity associated with this race for fundraising.\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"List of events within this race (e.g., 5K, 10K, Half Marathon).\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Event\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Event\": {\n      \"type\": \"object\",\n      \"description\": \"A specific event distance or category within a race. Participants register for a specific event.\",\n      \"required\": [\"event_id\", \"name\"],\n      \"properties\": {\n        \"event_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique event identifier within the race.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Event name (e.g., '5K Run', '10K Walk', 'Half Marathon').\"\n        },\n        \"start_time\": {\n        \
  \  \"type\": \"string\",\n          \"description\": \"Event start time in the race's local timezone.\"\n        },\n        \"end_time\": {\n          \"type\": \"string\",\n          \"description\": \"Event end time.\"\n        },\n        \"distance\": {\n          \"type\": \"number\",\n          \"description\": \"Event distance value.\",\n          \"minimum\": 0\n        },\n        \"distance_unit\": {\n          \"type\": \"string\",\n          \"description\": \"Unit for the distance value.\",\n          \"enum\": [\"K\", \"M\", \"Miles\"]\n        },\n        \"max_participants\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of participants allowed. Null means unlimited.\",\n          \"minimum\": 0\n        },\n        \"registration_opens\": {\n          \"type\": \"string\",\n          \"description\": \"Date/time when registration opens for this event.\"\n        },\n        \"registration_closes\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"Date/time when registration closes for this event.\"\n        },\n        \"age_min\": {\n          \"type\": \"integer\",\n          \"description\": \"Minimum age requirement.\",\n          \"minimum\": 0\n        },\n        \"age_max\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum age requirement.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"Participant\": {\n      \"type\": \"object\",\n      \"description\": \"A registered participant in a race event.\",\n      \"required\": [\"registration_id\"],\n      \"properties\": {\n        \"registration_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique registration identifier.\"\n        },\n        \"user_id\": {\n          \"type\": \"integer\",\n          \"description\": \"RunSignup user account ID.\"\n        },\n        \"first_name\": {\n          \"type\": \"string\"\n        },\n        \"last_name\": {\n          \"type\"\
  : \"string\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\"\n        },\n        \"dob\": {\n          \"type\": \"string\",\n          \"description\": \"Date of birth in MM/DD/YYYY format.\"\n        },\n        \"gender\": {\n          \"type\": \"string\",\n          \"enum\": [\"M\", \"F\", \"X\"]\n        },\n        \"bib_num\": {\n          \"type\": \"string\",\n          \"description\": \"Assigned bib number.\"\n        },\n        \"chip_num\": {\n          \"type\": \"string\",\n          \"description\": \"Assigned RFID chip number.\"\n        },\n        \"event_id\": {\n          \"type\": \"integer\"\n        },\n        \"event_name\": {\n          \"type\": \"string\"\n        },\n        \"race_id\": {\n          \"type\": \"integer\"\n        },\n        \"registration_date\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"Result\": {\n      \"type\": \"\
  object\",\n      \"description\": \"A race result entry for a participant including place and finish time.\",\n      \"required\": [\"registration_id\"],\n      \"properties\": {\n        \"result_id\": {\n          \"type\": \"integer\"\n        },\n        \"registration_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Links this result to the participant's registration.\"\n        },\n        \"bib_num\": {\n          \"type\": \"string\"\n        },\n        \"clock_time\": {\n          \"type\": \"string\",\n          \"description\": \"Gun time from start (HH:MM:SS.ms format).\"\n        },\n        \"chip_time\": {\n          \"type\": \"string\",\n          \"description\": \"Net chip time from crossing start line (HH:MM:SS.ms format).\"\n        },\n        \"place_overall\": {\n          \"type\": \"integer\",\n          \"description\": \"Overall finish place across all genders and ages.\",\n          \"minimum\": 1\n        },\n        \"place_gender\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Finish place within the participant's gender category.\",\n          \"minimum\": 1\n        },\n        \"place_division\": {\n          \"type\": \"integer\",\n          \"description\": \"Finish place within the participant's age/gender division.\",\n          \"minimum\": 1\n        },\n        \"pace\": {\n          \"type\": \"string\",\n          \"description\": \"Pace per mile or kilometer (MM:SS format).\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/runsignup/refs/heads/main/json-schema/runsignup-race-schema.json
tags:
- Race Registration
- Event Management
- Running
- Sports
- Fitness
- Timing
- Fundraising
title: RunSignup Race
---
