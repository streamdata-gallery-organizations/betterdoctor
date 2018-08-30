{
  "info": {
    "name": "BetterDoctor Retrieve a specific practice description using NPI",
    "_postman_id": "14940b99-ce59-4ace-b022-c09376d9c1fa",
    "description": "Returns a practice object based on an NPI. The office returned is registered in the NPI directory. There may be additional offices with this NPI registered at this location. Use the /practices search to find additional locations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Doctor",
      "item": [
        {
          "id": "eb51eb74-b4ba-402d-87f8-10bf227ac7c7",
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
              "id": "f44fcba6-f126-47ed-a298-ae2791af83e6"
            }
          ]
        }
      ]
    },
    {
      "name": "Doctors",
      "item": [
        {
          "id": "5837e0c1-caf7-4fa0-8edb-8e1fc397d5d3",
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
              "id": "4c13b8cc-33d2-4cc4-b64b-7c5ff1fc43a9"
            }
          ]
        },
        {
          "id": "bb09345c-c875-4357-8396-afa1a7217124",
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
              "id": "72a8582b-8b1c-4f72-9f39-0f54829302e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Practices",
      "item": [
        {
          "id": "d0c39c3e-d4e7-4a76-a26c-fe0280a07c87",
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
              "id": "73008d8b-f5e4-4bf6-bb09-eab19692cc88"
            }
          ]
        },
        {
          "id": "d5534ab3-b891-479a-95ca-fecb7af1eb9e",
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
              "id": "fa182677-df5b-40df-ad10-78560e91bcfa"
            }
          ]
        },
        {
          "id": "b5db338b-e84f-48e1-bae3-3654d7734737",
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
              "id": "e38bcbe1-f0dd-4086-8bec-0565523c679a"
            }
          ]
        }
      ]
    }
  ]
}