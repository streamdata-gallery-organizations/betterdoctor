{
  "info": {
    "name": "BetterDoctor Retrieve a list of doctors in this practice.",
    "_postman_id": "4b2a6a20-c8a3-490e-9c65-149dc83fb78a",
    "description": "Returns a paginated list of doctors in the specified practice. This is a convenience endpoint, you may also use /doctors search for all doctors.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Doctor",
      "item": [
        {
          "id": "9e7f6b1e-314b-4d4a-a1aa-a48f18725629",
          "name": "doctor-search",
          "request": {
            "url": "http://api.betterdoctor.com/2016-03-01/doctors?fields=%7B%7D&first_name=%7B%7D&gender=%7B%7D&insurance_uid=%7B%7D&last_name=%7B%7D&limit=%7B%7D&location=%7B%7D&name=%7B%7D&practice_uid=%7B%7D&query=%7B%7D&skip=%7B%7D&sort=%7B%7D&specialty_uid=%7B%7D&user_key=%7B%7D&user_location=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Doctor search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3b4cdf3-f73d-4a3d-aa9e-3d68f36cab65"
            }
          ]
        }
      ]
    },
    {
      "name": "Doctors",
      "item": [
        {
          "id": "da6e5edd-8364-48d1-97ff-e536e3a1eb35",
          "name": "returns-a-doctor-object-based-on-an-uid-or-a-slug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.betterdoctor.com",
              "path": [
                "2016-03-01",
                "doctors/:uid"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "uid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a doctor object based on an uid or a slug"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c844fa10-b316-4662-a671-5534a1aa50e8"
            }
          ]
        },
        {
          "id": "9e9c7e1d-2579-498c-8923-153611699e7d",
          "name": "returns-a-doctor-object-using-npi",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.betterdoctor.com",
              "path": [
                "2016-03-01",
                "doctors/npi/:npi"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "npi",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a doctor object using NPI"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c989ed3b-7670-4679-81af-1a595bdde256"
            }
          ]
        }
      ]
    },
    {
      "name": "Practices",
      "item": [
        {
          "id": "a846ab6f-1ad3-427f-a6e7-13897e969459",
          "name": "results-are-provider-service-locations-commonly-referred-as-practices-or-doctors-offices",
          "request": {
            "url": "http://api.betterdoctor.com/2016-03-01/practices?fields=%7B%7D&limit=%7B%7D&location=%7B%7D&name=%7B%7D&skip=%7B%7D&sort=%7B%7D&user_key=%7B%7D&user_location=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Results are provider service locations, commonly referred as practices or doctor's offices."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f73b0370-7383-4e81-abc6-51d2ec32525b"
            }
          ]
        },
        {
          "id": "86754c3c-d9cc-446b-ae4f-be2ae904eb64",
          "name": "returns-a-practice-object-based-on-an-uid-or-a-slug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.betterdoctor.com",
              "path": [
                "2016-03-01",
                "practices/:uid"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "uid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a practice object based on an uid or a slug"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "656ea653-f4b5-4b5b-9c08-0a039cfbd7ba"
            }
          ]
        },
        {
          "id": "330d293b-ea6d-4493-9ed8-aafd513f1158",
          "name": "returns-a-practice-object-based-on-an-npi-the-office-returned-is-registered-in-the-npi-directory-the",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.betterdoctor.com",
              "path": [
                "2016-03-01",
                "practices/npi/:npi"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "npi",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a practice object based on an NPI. The office returned is registered in the NPI directory. There may be additional offices with this NPI registered at this location. Use the /practices search to find additional locations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30a2cc8f-ce9d-419a-91ad-e57fc5654ed9"
            }
          ]
        },
        {
          "id": "90510440-1e53-46b2-973d-90e69370f97e",
          "name": "returns-a-paginated-list-of-doctors-in-the-specified-practice-this-is-a-convenience-endpoint-you-may",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.betterdoctor.com",
              "path": [
                "2016-03-01",
                "practices/:uid/doctors"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "uid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated list of doctors in the specified practice. This is a convenience endpoint, you may also use /doctors search for all doctors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c89d98c1-cf1c-41be-b3da-db51583eb2d9"
            }
          ]
        }
      ]
    }
  ]
}