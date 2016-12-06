# Eventhub to app insights pipe

This is a general eventhubs to app insights consumer. The idea it is that you would use this to pipe events from event hubs to application insights.

## How to use it

To use this just deploy this to your webjob you would need to change the config file to something that it is compatible with the following config.

the config file config.json must be placed on the same folder of the webjob.

```
{
    "Eventhub": {
        "connectionstring": ""
        "path": ""
    }
    ApplicationInsights : [
        {
            "types": [
                "type.to.be.used"
            ]
            "applicationId": "insights"
        },
        {
            "types": [
                "other.types.to.be.used",
                "some.other.type.used"
            ]
            "applicationId": "insights2"
        }
    ]
}
```