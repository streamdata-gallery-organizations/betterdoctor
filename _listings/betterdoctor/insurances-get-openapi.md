---
swagger: "2.0"
x-collection-name: BetterDoctor
x-complete: 0
info:
  title: BetterDoctor Retrieve insurance providers and plans
  description: Insurance provider & plan list
  version: 1.0.0
host: api.betterdoctor.com
basePath: /2016-03-01
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /doctors:
    get:
      summary: Doctor search
      description: Doctor search
      operationId: doctor-search
      x-api-path-slug: doctors-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: first_name
        description: The doctors first name; partial (type-ahead) characters/names
          are accepted
      - in: query
        name: gender
        description: The doctors gender (male or female)
      - in: query
        name: insurance_uid
        description: UID of an insurance plan (e
      - in: query
        name: last_name
        description: The doctors last name; partial (type-ahead) characters/names
          are accepted
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: location
        description: Search area - Either Circular (lat,lon,range (miles)) or Bounding
          box (top-right, bottom-left) (lat,lon,lat,lon)
      - in: query
        name: name
        description: The doctors name; searches in both first and last names
      - in: query
        name: practice_uid
        description: BetterDoctor Practice UID
      - in: query
        name: query
        description: Search all fields by a keyword query (e
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: sort
        description: 'Sort order for the search results (full-name-asc: Alphabetical
          sort by full provider name ascending'
      - in: query
        name: specialty_uid
        description: UID of a specialty (e
      - in: query
        name: user_key
        description: Your API access key
      - in: query
        name: user_location
        description: Users current location
      responses:
        200:
          description: OK
      tags:
      - Doctor
      - Search
  /doctors/{uid}:
    get:
      summary: Retrieve a specific doctor description
      description: Returns a doctor object based on an uid or a slug
      operationId: returns-a-doctor-object-based-on-an-uid-or-a-slug
      x-api-path-slug: doctorsuid-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: path
        name: uid
        description: BetterDoctor Doctor UID
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Doctors
  /doctors/npi/{npi}:
    get:
      summary: Retrieve a specific doctor description using NPI
      description: Returns a doctor object using NPI
      operationId: returns-a-doctor-object-using-npi
      x-api-path-slug: doctorsnpinpi-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: path
        name: npi
        description: The National Provider Identifier of the doctor to retrieve
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Doctors
  /practices:
    get:
      summary: Practice Search
      description: Results are provider service locations, commonly referred as practices
        or doctor's offices.
      operationId: results-are-provider-service-locations-commonly-referred-as-practices-or-doctors-offices
      x-api-path-slug: practices-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: location
        description: Search area - Either Circular (lat,lon,range (miles)) or Bounding
          box (top-right, bottom-left) (lat,lon,lat,lon)
      - in: query
        name: name
        description: "The practice\u2019s name"
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: sort
        description: 'Sort order for the search results (full-name-asc: Alphabetical
          sort by full provider name ascending'
      - in: query
        name: user_key
        description: Your API access key
      - in: query
        name: user_location
        description: 'Users current location: lat, lon'
      responses:
        200:
          description: OK
      tags:
      - Practices
      - Search
  /practices/{uid}:
    get:
      summary: Retrieve a specific practice description
      description: Returns a practice object based on an uid or a slug
      operationId: returns-a-practice-object-based-on-an-uid-or-a-slug
      x-api-path-slug: practicesuid-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: path
        name: uid
        description: BetterDoctor Practice UID
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Practices
  /practices/npi/{npi}:
    get:
      summary: Retrieve a specific practice description using NPI
      description: Returns a practice object based on an NPI. The office returned
        is registered in the NPI directory. There may be additional offices with this
        NPI registered at this location. Use the /practices search to find additional
        locations.
      operationId: returns-a-practice-object-based-on-an-npi-the-office-returned-is-registered-in-the-npi-directory-the
      x-api-path-slug: practicesnpinpi-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: path
        name: npi
        description: National Provider Identifier (NPI)
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Practices
  /practices/{uid}/doctors:
    get:
      summary: Retrieve a list of doctors in this practice.
      description: Returns a paginated list of doctors in the specified practice.
        This is a convenience endpoint, you may also use /doctors search for all doctors.
      operationId: returns-a-paginated-list-of-doctors-in-the-specified-practice-this-is-a-convenience-endpoint-you-may
      x-api-path-slug: practicesuiddoctors-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: path
        name: uid
        description: BetterDoctor Practice UID
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Practices
      - Doctors
  /practices/npi/{npi}/doctors:
    get:
      summary: Retrieve a list of doctors in this practice using NPI
      description: Returns a paginated list of doctors in the specified practice.
        This is a convenience endpoint, you may also use /doctors search for all doctors.
      operationId: returns-a-paginated-list-of-doctors-in-the-specified-practice-this-is-a-convenience-endpoint-you-may
      x-api-path-slug: practicesnpinpidoctors-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: path
        name: npi
        description: National Provider Identifier (NPI)
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Practices
      - Doctors
  /specialties:
    get:
      summary: Retrieve a list of all specialties
      description: Specialty group list
      operationId: specialty-group-list
      x-api-path-slug: specialties-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Specialties
  /insurances:
    get:
      summary: Retrieve insurance providers and plans
      description: Insurance provider & plan list
      operationId: insurance-provider--plan-list
      x-api-path-slug: insurances-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Insurance
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---