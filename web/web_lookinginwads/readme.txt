querying 


will return the schemas

{
                            "name": "super_super_secret_flag_dispenser",
                            "description": null,
                            "args": [
                                {
                                    "name": "authorized",
                                    "description": null,
                                    "type": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "SCALAR",
                                            "name": "Boolean",
                                            "ofType": null
                                        }
                                    },
                                    "defaultValue": null
                                }
                            ],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "String",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        }

query {
    super_super_secret_flag_dispenser(authorized: true)
}

will return the flag

{
    "data": {
        "super_super_secret_flag_dispenser": "MetaCTF{look_deep_and_who_knows_what_you_might_find}"
    }
}