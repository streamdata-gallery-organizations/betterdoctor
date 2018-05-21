{
  "info": {
    "name": "BetterDoctor Retrieve a list of doctors in this practice using NPI",
    "_postman_id": "5266fe2a-537c-4bc4-9837-ac740c6210b7",
    "description": "Returns a paginated list of doctors in the specified practice. This is a convenience endpoint, you may also use /doctors search for all doctors.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Doctor",
      "item": [
        {
          "id": "a3316dc3-2294-4556-a539-bfb19f7aeef2",
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
              "id": "390f38fa-b077-4b1b-91c4-d45493d1173b"
            }
          ]
        }
      ]
    },
    {
      "name": "Doctors",
      "item": [
        {
          "id": "9366ea30-312e-4ec2-82d6-dd6a6b8aafaf",
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
              "id": "124e17a8-74dc-420e-a6a3-31d51682f234"
            }
          ]
        },
        {
          "id": "f0028e86-1e4f-4656-82c1-c6ac37e18894",
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
              "id": "9cafac00-a4f9-405d-8e53-7c8c6dd82af3"
            }
          ]
        }
      ]
    },
    {
      "name": "Practices",
      "item": [
        {
          "id": "29ce7505-c46e-4c0c-a22f-1594cf84051e",
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
              "id": "241cb193-4228-475c-a745-e6f22b8860a9"
            }
          ]
        },
        {
          "id": "2e8c27d0-6764-45b0-a746-04238f09fd77",
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
              "id": "b36747fc-8faf-4d3d-859d-2729e15c0203"
            }
          ]
        },
        {
          "id": "7bd72166-5d59-4a9c-87c4-f2d8571e4403",
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
              "id": "ef8503cb-b7fb-431c-b7d7-114f7a575923"
            }
          ]
        },
        {
          "id": "d757100f-5bd7-49f9-a03f-4bc05fc828ba",
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
              "id": "f8970833-09f3-4fd2-a49c-112d622d8339"
            }
          ]
        },
        {
          "id": "24bed602-b5a9-414b-aead-050c6e505aba",
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
              "id": "811a757b-1714-4c10-866f-409151e2d9e8"
            }
          ]
        }
      ]
    }
  ]
}