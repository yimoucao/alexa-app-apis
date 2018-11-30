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

# `/api/devices-v2/`

# `/api/devices-v2/device?cached=false`

# `/api/devices/`

# `/api/devices/{ALEXA_DEVICE_TYPE_GROUP}/` + d.serial + `?deviceType=`

# `/api/eon/householdaccounts`

# `/api/external-auth`

# `/api/external-auth/link-url`

# `/api/get-available-countries-for-connect`

# `/api/get-customer-pfm`

# `/api/get-languages`

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

