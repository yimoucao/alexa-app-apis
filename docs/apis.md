APIs


# `/api/allowed-providers`

Response:

    {
        "allowedProviders": ["MUSIC_SKILL","SPOTIFY","AMAZON_MUSIC",...]
    }

# `/api/authentication`

# `/api/available-mid-field`

Response:

    {
        "midFieldStates":null
    }

# `/api/bluetooth`

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

# `/api/bluetooth/cancel-pairing-mode`

# `/api/bluetooth/disconnect-sink/{k}/`

# `/api/bluetooth/initiate-scan-for-sinks`

# `/api/bluetooth/initiate-scan-for-sinks/{deviceTypeId}/{deviceSerialNumber}`

# `/api/bluetooth/pair-sink/{s}/`

# `/api/bluetooth/unpair-sink/`

# `/api/bluetooth/unpair-sink/{deviceTypeId}/{deviceSerialNumber}`

# `/api/calendar/account`

# `/api/communications`

# `/api/customer-status`

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

# `/api/devices-v2/device`

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

# `/api/devices/`

# `/api/devices/{ALEXA_DEVICE_TYPE_GROUP}/` + d.serial + `?deviceType=`

# `/api/eon/householdaccounts`

# `/api/external-auth`

# `/api/external-auth/link-url`

# `/api/get-available-countries-for-connect`

Response:

    {
    "availableCountries": [
        {
        "countryCode": "DE",
        "dialingCode": "+49"
        },
        {
        "countryCode": "GI",
        "dialingCode": "+350"
        },
        {
        "countryCode": "AT",
        "dialingCode": "+43"
        },
        {
        "countryCode": "GB",
        "dialingCode": "+44"
        },
        {
        "countryCode": "IE",
        "dialingCode": "+353"
        },
        {
        "countryCode": "US",
        "dialingCode": "+1"
        }
    ]
    }


# `/api/get-customer-pfm`

Get customer's personal finantial market (?)

TODO: all market place ids

Response:

    {
    "countryOfResidence": "US",
    "effectiveMarketPlaceId": "XXXXXXXXXXXXX",
    "marketPlaceDomainName": "https://www.amazon.com",
    "marketPlaceId": "XXXXXXXXXXXXX",
    "marketPlaceLocale": "en-US"
    }

# `/api/get-languages`

return available languages. Currently supported locales: de-DE, en-US, en-CA, en-IN, es-ES, es-MX, it-IT, en-AU, fr-FR, en-GB, ja-JP

Response:

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
        {
        "languageCountryCode": "CA",
        "languageName": "English (Canada)",
        "locale": "en-CA"
        },
        ...
    ]
    }



# `/api/household/CSRFToken?householdOperationName=` + a + `;sessionId=`

# `/api/iheartradio/preferences`

# `/api/iheartradio/registration-code`

# `/api/lemur`

# `/api/lemur/access/`

# `/api/lemur/conspiracy`

# `/api/lemur/conspiracy2`

# `/api/lists/fetchUserPreference`

# `/api/lists/linkedPartners`

# `/api/lists/listPartners`

# `/api/music-household`

# `/api/photos/get-profile`

# `/api/ping`

Response:

    healthy

# `/api/poptart/default-device`

# `/api/prime/get-prime-free-trial-eligibility`

# `/api/prime/get-prime-free-trial-offer?locationID=`

# `/api/provider-preferences`

# `/api/resolve-device-address-v2`

# `/api/salmon/preferences`

# `/api/speakers/music-linking`

# `/api/traffic/settings`

# `/api/tts/audio/data`

# `/api/tvlistings/settings`

# `/api/utterance/audio/data`

# `/api/utterance/audio/data?id=`

# `/api/verify-account`

# `/api/video/` + this.deviceType + `/`

# `/api/wake-word`

Response:

    {"wakeWords":[]}

# `/api/wake-words-downloaded`

Response:

    {"message":null}

# `/api/wake-words-locale`

Response:

    {"message":null}

