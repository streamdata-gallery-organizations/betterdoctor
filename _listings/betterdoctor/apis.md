---
name: BetterDoctor
x-slug: betterdoctor
description: BetterDoctor helps people find and connect to the best doctors through
  our consumer app, doctor marketing services, and API. Our mission is to help increase
  transparency in healthcare and help consumers make better decisions.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
x-kinRank: "8"
x-alexaRank: "625342"
tags: BetterDoctor
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/apis.md
specificationVersion: "0.14"
apis:
- name: BetterDoctor Doctor search
  x-api-slug: betterdoctor
  description: Doctor search
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//doctors
  tags: Doctor, Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/doctors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/doctors-get-openapi.md
- name: BetterDoctor Retrieve a specific doctor description
  x-api-slug: betterdoctor
  description: Returns a doctor object based on an uid or a slug
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//doctors/{uid}
  tags: Doctors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/doctorsuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/doctorsuid-get-openapi.md
- name: BetterDoctor Retrieve a specific doctor description using NPI
  x-api-slug: betterdoctor
  description: Returns a doctor object using NPI
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//doctors/npi/{npi}
  tags: Doctors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/doctorsnpinpi-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/doctorsnpinpi-get-openapi.md
- name: BetterDoctor Practice Search
  x-api-slug: betterdoctor
  description: Results are provider service locations, commonly referred as practices
    or doctor's offices.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//practices
  tags: Practices, Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/practices-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/practices-get-openapi.md
- name: BetterDoctor Retrieve a specific practice description
  x-api-slug: betterdoctor
  description: Returns a practice object based on an uid or a slug
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//practices/{uid}
  tags: Practices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/practicesuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/practicesuid-get-openapi.md
- name: BetterDoctor Retrieve a specific practice description using NPI
  x-api-slug: betterdoctor
  description: Returns a practice object based on an NPI. The office returned is registered
    in the NPI directory. There may be additional offices with this NPI registered
    at this location. Use the /practices search to find additional locations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//practices/npi/{npi}
  tags: Practices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/practicesnpinpi-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/practicesnpinpi-get-openapi.md
- name: BetterDoctor Retrieve a list of doctors in this practice.
  x-api-slug: betterdoctor
  description: Returns a paginated list of doctors in the specified practice. This
    is a convenience endpoint, you may also use /doctors search for all doctors.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//practices/{uid}/doctors
  tags: Practices,Doctors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/practicesuiddoctors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/practicesuiddoctors-get-openapi.md
- name: BetterDoctor Retrieve a list of doctors in this practice using NPI
  x-api-slug: betterdoctor
  description: Returns a paginated list of doctors in the specified practice. This
    is a convenience endpoint, you may also use /doctors search for all doctors.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//practices/npi/{npi}/doctors
  tags: Practices,Doctors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/practicesnpinpidoctors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/practicesnpinpidoctors-get-openapi.md
- name: BetterDoctor Retrieve a list of all specialties
  x-api-slug: betterdoctor
  description: Specialty group list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//specialties
  tags: Specialties
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/specialties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/specialties-get-openapi.md
- name: BetterDoctor Retrieve insurance providers and plans
  x-api-slug: betterdoctor
  description: Insurance provider & plan list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//insurances
  tags: Insurance
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/insurances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/insurances-get-openapi.md
- name: BetterDoctor Retrieve a list of known conditions
  x-api-slug: betterdoctor
  description: List all conditions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//conditions
  tags: Conditions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/conditions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/conditions-get-openapi.md
- name: BetterDoctor Add a new record
  x-api-slug: betterdoctor
  description: "Creates validation document using the request body, and returns the
    document created with unique identifier in Location header for reference. This
    is how validation data is submitted to BetterDoctor for addition to the API. The
    posted document must conform to BetterDoctor\u2019s JSON schema for validation
    objects, see included model specification for more information. <br><h4 style='margin-bottom:
    0px !important;'> Return Headers </h4> <div>Location: The uid of the created document.
    This can be used to access the document again without executing a search.</div>"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//validations
  tags: Record, Search, Validations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/validations-post-openapi.md
- name: BetterDoctor Record search
  x-api-slug: betterdoctor
  description: "The endpoint can be used to identify providers with validation data.
    The search supports BetterDoctor unique provider identifier, National Provider
    Identifier (NPI) or reference uid based provider lookups. BetterDoctor identifiers
    and NPIs for doctors and practices can be discovered using BetterDoctor API\u2019s
    search functionalities. <br><h4 style='margin-bottom: 0px !important;'> Return
    Headers </h4> <div>Last-Modified: Timestamp of the last validation made over the
    matching validations. The value can be used to query changes in the validation
    status for the provider using since parameter in collaboration with HEAD method.</div>"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//validations
  tags: Record, Search, Validations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/validations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/validations-get-openapi.md
- name: BetterDoctor Check if new records exists
  x-api-slug: betterdoctor
  description: 'The endpoint can be used to identify providers with validation data,
    and discover changes. It providers search functionalities like its GET method
    alternative, but does not return any validation data. Instead of the data itself,
    it returns 200 OK if matching validation documents based on the given query are
    found. And it returns 304 if no validation documents are found after the timestamp
    given using If-Modified-Since HTTP header or since parameter. <br><h4 style=''margin-bottom:
    0px !important;''> Return Headers </h4> <div>Last-Modified: Timestamp of the last
    validation made over the matching validations. </div>'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//validations
  tags: Record, Search, Validations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/validations-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/validations-head-openapi.md
- name: BetterDoctor Retrieve a specific record
  x-api-slug: betterdoctor
  description: 'Returns requested validation document. The endpoint is a conveniece
    method to check status and accepted data of a specific validation, like after
    creation of a validation. The response consist of raw data from the validation
    event and related validation information. <br><h4 style=''margin-bottom: 0px !important;''>
    Return Headers </h4> <div>Last-Modified: Timestamp of the validation made.</div>'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//validations/{uid}
  tags: Record, Search, Validations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/validationsuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/validationsuid-get-openapi.md
- name: BetterDoctor Check if a specific record exists
  x-api-slug: betterdoctor
  description: 'The endpoint can be used to discover if a validation document exists
    in the API. <br><h4 style=''margin-bottom: 0px !important;''> Return Headers </h4>
    <div>Last-Modified: Timestamp of the validation made.</div>'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//validations/{uid}
  tags: Record, Search, Validations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/validationsuid-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/validationsuid-head-openapi.md
- name: BetterDoctor API Health Check
  x-api-slug: betterdoctor
  description: Returns basic API health information for monitoring
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01//info
  tags: API, Health, Check
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/info-get-openapi.md
- name: BetterDoctor
  x-api-slug: betterdoctor
  description: BetterDoctor helps people find and connect to the best doctors through
    our consumer app, doctor marketing services, and API. Our mission is to help increase
    transparency in healthcare and help consumers make better decisions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01
  tags: BetterDoctor
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/betterdoctor/master/_listings/betterdoctor/openapi.md
x-common:
- type: x-blog
  url: https://betterdoctor.com/health/
- type: x-blog-rss
  url: https://betterdoctor.com/health/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/betterdoctor-inc
- type: x-developer
  url: https://developer.betterdoctor.com
- type: x-email
  url: hello@betterdoctor.com
- type: x-email
  url: press@betterdoctor.com
- type: x-email
  url: tony@betterdoctor.com
- type: x-email
  url: privacy@betterdoctor.com
- type: x-email
  url: support@betterdoctor.com
- type: x-email
  url: copyright@betterdoctor.com
- type: x-github
  url: https://github.com/betterdoctor
- type: x-twitter
  url: https://twitter.com/betterdoctor
- type: x-website
  url: https://betterdoctor.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---