{
  "info": {
    "name": "BetterDoctor Retrieve a list of all specialties",
    "_postman_id": "a21d18a3-7e7e-4712-983e-13f18a1903d8",
    "description": "Specialty group list",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Doctor",
      "item": [
        {
          "id": "8f456b44-978f-4515-bcee-49fef4c28e1c",
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
              "id": "d956536c-ce60-4fc9-89b1-1c9b9f2c6b15"
            }
          ]
        }
      ]
    },
    {
      "name": "Doctors",
      "item": [
        {
          "id": "0aa85751-6020-4e94-a332-e046c7f47027",
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
              "id": "81d5f2fd-dea5-4690-921b-1380a3630906"
            }
          ]
        },
        {
          "id": "05a652b4-e195-4597-a8ea-64e48504819f",
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
              "id": "bfd2b404-3271-4243-834b-55955b0e844a"
            }
          ]
        }
      ]
    },
    {
      "name": "Practices",
      "item": [
        {
          "id": "ce1420b5-efd9-4d88-92c9-65b4855314f0",
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
              "id": "90d11f1b-278d-4636-974c-5f9bf101d6f6"
            }
          ]
        },
        {
          "id": "520e4185-761e-4e13-b146-b729d9a0c57e",
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
              "id": "c1ec01c7-9227-417d-8157-731935ed6116"
            }
          ]
        },
        {
          "id": "469751c0-1d04-4981-9e46-2a4d739129a4",
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
              "id": "51b0cb69-1c2b-4e60-a2b6-faf0a638081d"
            }
          ]
        },
        {
          "id": "fa78ad39-300f-4295-9408-e44b7cdffcda",
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
              "id": "5d8ee66c-ecdc-447f-9947-918f577883cd"
            }
          ]
        },
        {
          "id": "fb5a4de3-764e-4818-aeb2-7e04c2bd6614",
          "name": "returns-a-paginated-list-of-doctors-in-the-specified-practice-this-is-a-convenience-endpoint-you-may",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.betterdoctor.com",
              "path": [
                "2016-03-01",
                "practices/npi/:npi/doctors"
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
            "description": "Returns a paginated list of doctors in the specified practice. This is a convenience endpoint, you may also use /doctors search for all doctors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19161d29-b6f8-46b7-8f1a-8db135a7c801"
            }
          ]
        }
      ]
    },
    {
      "name": "Specialties",
      "item": [
        {
          "id": "bc7a4c62-e302-476c-918f-4b63a786bbbc",
          "name": "specialty-group-list",
          "request": {
            "url": "http://api.betterdoctor.com/2016-03-01/specialties?fields=%7B%7D&limit=%7B%7D&skip=%7B%7D&user_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specialty group list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6838cd0a-f19a-4813-beed-403994d73912"
            }
          ]
        }
      ]
    }
  ]
}