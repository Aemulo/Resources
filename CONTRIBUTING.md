# Contributing Resources

There are currently two types of resources that can be contributed to Aemulo, image rules and localizations.

## Image Rules
Image rules are stored in `TagRules.json` and follow this schema:
``` 
{
    "manufacturer": UInt8? // The first byte of a UID, represents the manufacturer of the tag
    "type": String? // The type of tag it is
    "url": String? // A URL/host that can be found in any of the NDEF records on the tag

    "symbol": String // The name of an SF Symbol to replace the stock tag symbol. If the tag is not available for an older iOS version it will default back to stock.
}
```

## Localization
Localization for Aemulo now uses the updated Xcode 15 bundle format. To contribute and edit it is strongly recommended you open the bundle with Xcode 15 and add or modify the strings for your preferred language. 