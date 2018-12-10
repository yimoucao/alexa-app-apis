APIs

# Devices

## `/api/devices-v2/device`

GET parameters:

| parameter | value/description | required |
| --------- | ----------------- | -------- |
| cached    | false             | no       |

Response:

    {
    "devices": [
        {
        "accountName": "Echo Dot",
        "appDeviceList": [],
        "capabilities": [
            "SUPPORTS_SOFTWARE_VERSION",
            "AMAZON_MUSIC",
            "AUDIBLE",
            "VOLUME_SETTING",
            "MUSIC_SKILL",
            "DEREGISTER_DEVICE",
            "SOUND_SETTINGS",
            "ACTIVE_AFTER_FRO",
            "CHANGE_NAME",
            "FAR_FIELD_WAKE_WORD",
            "TIMERS_AND_ALARMS",
            "LEMUR_ALPHA",
            "I_HEART_RADIO",
            "PAIR_REMOTE",
            "PAIR_BT_SINK",
            "VOICE_TRAINING",
            "TAHOE_BYOD",
            "DREAM_TRAINING",
            "SLEEP",
            "PANDORA",
            "SET_LOCALE",
            "AUDIO_PLAYER",
            "GADGETS",
            "POPTART",
            "UPDATE_WIFI",
            "DS_VOLUME_SETTING",
            "TUNE_IN",
            "KINDLE_BOOKS",
            "FLASH_BRIEFING",
            "SALMON",
            "SUPPORTS_CONNECTED_HOME",
            "MICROPHONE",
            "SUPPORTS_CONNECTED_HOME_ALL",
            "CUSTOM_ALARM_TONE",
            "REMINDERS",
            "REQUIRES_OOBE_FOR_SETUP",
            "EARCONS",
            "PERSISTENT_CONNECTION",
            "GOLDFISH",
            "PAIR_BT_SOURCE",
            "DEREGISTER_FACTORY_RESET"
        ],
        "charging": null,
        "clusterMembers": [],
        "deviceAccountId": "XXXXXXXXXXXXX",
        "deviceFamily": "ECHO",
        "deviceOwnerCustomerId": "XXXXXXXXXXXXXX",
        "deviceType": "XXXXXXXXXXXXXX",
        "deviceTypeFriendlyName": null,
        "essid": null,
        "language": null,
        "macAddress": null,
        "online": false,
        "parentClusters": [],
        "postalCode": null,
        "registrationId": null,
        "remainingBatteryLevel": null,
        "serialNumber": "XXXXXXXXXXXXXXXX",
        "softwareVersion": "000000000"
        },
        {
        "accountName": "echosim_BETA",
        "appDeviceList": [],
        "capabilities": [
            "AMAZON_MUSIC",
            "AUDIBLE",
            "AUDIO_PLAYER",
            "VOLUME_SETTING",
            "MUSIC_SKILL",
            "DEREGISTER_DEVICE",
            "TUNE_IN",
            "CHANGE_NAME",
            "KINDLE_BOOKS",
            "TIMERS_AND_ALARMS",
            "MICROPHONE",
            "I_HEART_RADIO",
            "PEONY",
            "SUPPORTS_CONNECTED_HOME_CLOUD_ONLY",
            "DREAM_TRAINING",
            "PERSISTENT_CONNECTION",
            "GOLDFISH",
            "SLEEP"
        ],
        "charging": null,
        "clusterMembers": [],
        "deviceAccountId": "XXXXXXXXXXXXXX",
        "deviceFamily": "UNKNOWN",
        "deviceOwnerCustomerId": "XXXXXXXXXXXXXX",
        "deviceType": "XXXXXXXXXXXXXX",
        "deviceTypeFriendlyName": "echosim_BETA",
        "essid": null,
        "language": null,
        "macAddress": null,
        "online": false,
        "parentClusters": [],
        "postalCode": null,
        "registrationId": null,
        "remainingBatteryLevel": null,
        "serialNumber": "xxxxxx",
        "softwareVersion": "0"
        },
        ...
    ]
    }

## `/api/devices/`

## `/api/devices/{ALEXA_DEVICE_TYPE_GROUP}/` + d.serial + `?deviceType=`


# Alexa Preference

## `/api/allowed-providers`

Response:

    {
        "allowedProviders": ["MUSIC_SKILL","SPOTIFY","AMAZON_MUSIC",...]
    }

## `/api/provider-preferences`

Response:

    {
        "preferencesMap": {
            "MUSIC": [
                {
                    "associated": true,
                    "preferred": false,
                    "providerId": "AMAZON_MUSIC",
                    "providerName": "Amazon Music",
                    "skillId": null
                },
                {
                    "associated": true,
                    "preferred": true,
                    "providerId": "SPOTIFY",
                    "providerName": "Spotify",
                    "skillId": null
                }
            ],
            "STATION": [
                {
                    "associated": true,
                    "preferred": true,
                    "providerId": "AMAZON_MUSIC",
                    "providerName": "Amazon Music",
                    "skillId": null
                },
                {
                    "associated": true,
                    "preferred": false,
                    "providerId": "I_HEART_RADIO",
                    "providerName": "iHeartRadio",
                    "skillId": null
                }
            ]
        }
    }

## Communications

## `/api/communications/providers`

Response:

    {
    "cspList": [
        {
        "androidDeepLinkSupport": true,
        "cspUserId": "not-linked",
        "details": true,
        "iconUrl": "a/url/here",
        "id": "Lightyear",
        "launchUrl": "https://skype.com",
        "linked": false,
        "name": "Skype",
        "showWelcomeScreen": true,
        "usePrefMethodExtAuthIos": true
        }
        ...
    ]
    }



## `/api/tvlistings/settings`

Response:

    {
    "cableProvider": null,
    "providerNamesMap": {
        "AT&T U-verse": "AT&T U-verse",
        "Armstrong": "Armstrong",
        "Atlantic Broadband LLC": "Atlantic Broadband",
        "Broadstripe": "Broadstripe",
        "Cable ONE": "Cable ONE",
        "CenturyLink, Inc.": "CenturyLink",
        "Charter Communications": "Spectrum",
        "Comcast Corporation": "Comcast",
        "Cox Communications": "Cox",
        "DIRECTV": "DIRECTV",
        "Dish Network, LLC": "Dish",
        "Frontier Communications": "Frontier",
        "Google Fiber": "Google Fiber",
        "Mediacom LLC.": "Mediacom",
        "Midcontinent Cable Company": "Midco",
        "OPTIC Communications": "Optic HUB",
        "Service Electric Cable TV & Communications": "Service Electric",
        "Time Warner Cable": "Time Warner Cable",
        "Verizon FiOS": "FiOS",
        "WideOpenWest": "WOW! TV",
        "Windstream Communications": "Windstream"
    }
    }


## Flash Briefing (content)

## `/api/content-skills`

Return content skills the user has.

Response:

    {
        "contentSkills": [
            {
                "feeds": [
                    {
                        "feedId": {
                            "value": "793d6df5-6962-4e39-9eb0-8135c5015db8"
                        },
                        "imageUrl": "https://s3.amazonaws.com/CAPS-SSE/echo_developer/22a2ffe.d48b98d3.bda0ca22ce6c46d4b625ab4d9dd841ce/APP_ICON_LARGE?versionId=CcNqI.xPhATymJGMEoEa2SwtiSgV7aHN&AWSAccessKeyId=AKIAJFEYRBGIHK2BBYKA&Expires=1546984239&Signature=1jrhSvdNd8RnruTf1ucR9kLeyhk%3D",
                        "name": "Reuters Now",
                        "skillId": "amzn1.ask.skill.5ed629bb-1036-415b-986c-5d8e7042f3a2"
                    }
                ],
                "imageUrl": "https://s3.amazonaws.com/CAPS-SSE/echo_developer/88d1d934118242bc9921b951160f70e4/APP_ICON?versionId=tOAeK0QFR6bR6Rg4lhiLIDAqanXcn8kO&AWSAccessKeyId=AKIAJFEYRBGIHK2BBYKA&Expires=1546833438&Signature=LDlFQya%2B3V%2BOgThwr1ghZuu%2BI1U%3D",
                "name": "Reuters TV (U.S.)",
                "skillId": "amzn1.ask.skill.5ed629bb-1036-415b-986c-5d8e7042f3a2"
            },
            {
                "feeds": [
                    {
                        "feedId": {
                            "value": "a07ebb8e-73eb-4eec-a044-5905e975357c"
                        },
                        "imageUrl": "https://s3.amazonaws.com/CAPS-SSE/echo_developer/b8a1c2b3.d48b98d3.d72df964d707419e826aec46b4b5fdfc/APP_ICON_LARGE?versionId=dGujNHC7PiTTHbRAQ3FxZcW_7.GxWVmD&AWSAccessKeyId=AKIAJFEYRBGIHK2BBYKA&Expires=1546984170&Signature=9b8nzf8J0wpSMqrxbvy5igQIiZg%3D",
                        "name": "Today's Forecast",
                        "skillId": "amzn1.ask.skill.c86d0fa8-0307-471b-82af-aa71b816acc4"
                    }
                ],
                "imageUrl": "https://s3.amazonaws.com/CAPS-SSE/echo_developer/c1e8cd28e8814ebba2a25880f05db383/APP_ICON?versionId=GvRF5SR22UmX.O_v04zFK..44NI6kcQP&AWSAccessKeyId=AKIAJFEYRBGIHK2BBYKA&Expires=1546811531&Signature=w3xRSAbVwgqovodaui0ZGWsADy8%3D",
                "name": "Weather",
                "skillId": "amzn1.ask.skill.c86d0fa8-0307-471b-82af-aa71b816acc4"
            }
        ]
    }

## `/api/content-skills/enabled-feeds`

Methods: GET, POST

GET: Return content feeds the user enabled

Response:

    {
        "enabledFeeds": [
            {
                "feedId": {
                    "value": "793d6df5-6962-4e39-9eb0-8135c5015db8"
                },
                "imageUrl": "https://s3.amazonaws.com/CAPS-SSE/echo_developer/22a2ffe.d48b98d3.bda0ca22ce6c46d4b625ab4d9dd841ce/APP_ICON_LARGE?versionId=CcNqI.xPhATymJGMEoEa2SwtiSgV7aHN&AWSAccessKeyId=AKIAJFEYRBGIHK2BBYKA&Expires=1546984239&Signature=1jrhSvdNd8RnruTf1ucR9kLeyhk%3D",
                "name": "Reuters Now",
                "skillId": "amzn1.ask.skill.5ed629bb-1036-415b-986c-5d8e7042f3a2"
            },
            {
                "feedId": {
                    "value": "a07ebb8e-73eb-4eec-a044-5905e975357c"
                },
                "imageUrl": "https://s3.amazonaws.com/CAPS-SSE/echo_developer/b8a1c2b3.d48b98d3.d72df964d707419e826aec46b4b5fdfc/APP_ICON_LARGE?versionId=dGujNHC7PiTTHbRAQ3FxZcW_7.GxWVmD&AWSAccessKeyId=AKIAJFEYRBGIHK2BBYKA&Expires=1546984170&Signature=9b8nzf8J0wpSMqrxbvy5igQIiZg%3D",
                "name": "Today's Forecast",
                "skillId": "amzn1.ask.skill.c86d0fa8-0307-471b-82af-aa71b816acc4"
            }
        ]
    }

POST Params:

    "enabledFeeds": [
        {
        "feedId": { "value":  },
        "skillId": 
        },
        {
        "feedId": { "value":  },
        "skillId": 
        }
    ]


## FreeTime

## `/api/freeTime/childrenWithGrantedVpc`


## Traffic

## `/api/traffic/settings`

Methods: GET, POST

GET response:

    {
        "destination": {
            "addressId": "",
            "addressLine1": "",
            "addressLine2": "",
            "addressLine3": "",
            "city": "",
            "countryCode": "US",
            "county": "",
            "label": "`street` `city`, `state` `zipcode`",
            "placeId": null,
            "settingsAddressType": null,
            "state": "",
            "stationName": null,
            "street": "",
            "zipcode": ""
        },
        "origin": {
            "addressId": "",
            "addressLine1": "",
            "addressLine2": "",
            "addressLine3": "",
            "city": "",
            "countryCode": "US",
            "county": "",
            "label": "`street` `city`, `state` `zipcode`",
            "placeId": null,
            "settingsAddressType": null,
            "state": "",
            "stationName": null,
            "street": "",
            "zipcode": ""
        },
        "preferredTransportMode": "CAR",
        "transportNames": null,
        "waypoints": []
    }


POST params:


## `/api/traffic/suggest`

Methods: GET

GET params:

| param | value |
| ----- | ----- |
| q | some address |
| suggestionType | LOCATION_ADDRESS |

GET response:

    {
        "suggestionList": [
            {
                "internalLabel": "",
                "label": "",
                "placeId": null
            }
        ]
    }




## Lists

## `/api/lists/linkedPartners`

List linked list partners.

## `/api/lists/listPartners`

List TODO list partners. Such as: Any.do, AnyList, Cozi Lists, Picniic, Todoist.

Response:

    {
    "listPartners": [
        {
        "amazonStoreURL": null,
        "appId": "amzn1.ask.skill.5858c12a-c55c-4a1b-b59c-f7f6bfdf22ed",
        "appStoreURL": null,
        "linkingFlowAmazonDeepLinkURL": null,
        "linkingFlowAndroidDeepLinkURL": null,
        "linkingFlowIOSDeepLinkURL": null,
        "linkingFlowWebURL": "skills/dp/B074X3JRHL/?ref=skill_dsk_skb_sr_0",
        "logoImageURL": "https://images-na.ssl-images-amazon.com/images/I/41y53Nnp+wL.png",
        "name": "Any.do",
        "playStoreURL": null,
        "webURL": null
        },
        ...
    ]
    }



# General

## Voice Responses

## `api/voice-responses`

Methods: GET, POST

GET:

If brief mode is on, `TERSE` will be listed in `promptModes`

GET response:

    {
        "promptModes": []
    }

POST:


# TODO

## `/api/authentication`

## `/api/available-mid-field`

Response:

    {
        "midFieldStates":null
    }

## `/api/bluetooth`

Response:

    {
        "bluetoothStates":[
        {
            "deviceSerialNumber":"XXXXXXXXXXXXXXXX",
            "deviceType":"XXXXXXXXXXXXXX",
            "friendlyName":null,
            "gadgetPaired":false,
            "online":false,
            "pairedDeviceList":null,
            "sconeBattery":null,
            "sconePaired":false,
            "softwareVersion":"618622620",
            "streamingState":null
        },
        ...
        ]
    }

## `/api/bluetooth/cancel-pairing-mode`

## `/api/bluetooth/disconnect-sink/{k}/`

## `/api/bluetooth/initiate-scan-for-sinks`

## `/api/bluetooth/initiate-scan-for-sinks/{deviceTypeId}/{deviceSerialNumber}`

## `/api/bluetooth/pair-sink/{s}/`

## `/api/bluetooth/unpair-sink/`

## `/api/bluetooth/unpair-sink/{deviceTypeId}/{deviceSerialNumber}`

## `/api/calendar/account`


## `/api/customer-status`

Response:

    {
        "countryOfResidenceSet":true,
        "eulaAcceptance":true,
        "ftueSkipped":false,
        "hasActiveDopplers":true,
        "hasPhysical1PDevice":true,
        "preferredMarketplaceSet":true,
        "tutorialComplete":false
    }



## `/api/eon/householdaccounts`

## `/api/external-auth`

## `/api/external-auth/link-url`

## `/api/get-available-countries-for-connect`

Response:

| countryCode | dialingCode |
| ----------- | ----------- |
| DE          | +49         |
| GI          | +350        |
| AT          | +43         |
| GB          | +44         |
| IE          | +353        |
| US          | +1          |

    {
    "availableCountries": [
        {
        "countryCode": "DE",
        "dialingCode": "+49"
        },
        ...
    ]
    }


## `/api/get-customer-pfm`

Get customer's **p**ersonal **f**inantial **m**arket (?)

TODO: all market place ids

Response:

    {
    "countryOfResidence": "US",
    "effectiveMarketPlaceId": "XXXXXXXXXXXXX",
    "marketPlaceDomainName": "https://www.amazon.com",
    "marketPlaceId": "XXXXXXXXXXXXX",
    "marketPlaceLocale": "en-US"
    }

## `/api/get-languages`

return available languages. 

Currently supported locales: de-DE, en-US, en-CA, en-IN, es-ES, es-MX, it-IT, en-AU, fr-FR, en-GB, ja-JP

Response:

| languageCountryCode | languageName | locale |
| ------------------- | ------------ | ------ |
| DE | Deutsch      | de-DE |
| US | English (United States) | en-US |
| CA | English (Canada) | de-CA |
| CA | English (Canada) | de-CA |
| CA | English (Canada) | de-CA |
| CA | English (Canada) | de-CA |

    {
    "availableLanguages": [
        {
        "languageCountryCode": "DE",
        "languageName": "Deutsch",
        "locale": "de-DE"
        },
        {
        "languageCountryCode": "US",
        "languageName": "English (United States)",
        "locale": "en-US"
        },
        ...
    ]
    }



## `/api/household/CSRFToken?householdOperationName=` + a + `;sessionId=`

## `/api/iheartradio/preferences`

## `/api/iheartradio/registration-code`

## `/api/lemur`

## `/api/lemur/access/`

## `/api/lemur/conspiracy`

## `/api/lemur/conspiracy2`

## `/api/lists/fetchUserPreference`

Show user's list preference.

Response:

    {
        "customerListPreference": {
            "ShowDiscoverabilityPopup": false,
            "customerId": "XXXXXXXXXXXXXX"
        }
    }


## `/api/music-household`

Response:

    {
        "relationships": {
            "HAWKFIRE": {
                "currentRelationships": [],
                "pendingInvitations": [],
                "remainingInvites": 5,
                "selfRole": null,
                "suggestedRelationships": []
            }
        }
    }

## `/api/photos/get-profile`

## `/api/ping`

Response:

    healthy

## `/api/poptart/default-device`

## `/api/prime/get-prime-free-trial-eligibility`

## `/api/prime/get-prime-free-trial-offer?locationID=`

## `/api/resolve-device-address-v2`

## `/api/salmon/preferences`

## `/api/speakers/music-linking`



## `/api/tts/audio/data`

## `/api/tvlistings/settings`

## `/api/utterance/audio/data`

## `/api/utterance/audio/data?id=`

## `/api/verify-account`

## `/api/video/` + this.deviceType + `/`

## `/api/wake-word`

Response:

    {"wakeWords":[]}

## `/api/wake-words-downloaded`

Response:

    {"message":null}

## `/api/wake-words-locale`

Response:

    {"message":null}

