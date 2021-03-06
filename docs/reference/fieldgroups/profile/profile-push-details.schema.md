
# Push Notification Token Details Schema

```
https://ns.adobe.com/xdm/context/profile-push-details
```

Information regarding push notifications, such as mobile application and device details.

| [Abstract](../../../abstract.md) | [Extensible](../../../extensions.md) | [Status](../../../status.md) | [Identifiable](../../../id.md) | [Custom Properties](../../../extensions.md) | [Additional Properties](../../../extensions.md) | Defined In |
|----------------------------------|--------------------------------------|------------------------------|--------------------------------|---------------------------------------------|-------------------------------------------------|------------|
| Can be instantiated | Yes | Deprecated | No | Forbidden | Permitted | [fieldgroups/profile/profile-push-details.schema.json](fieldgroups/profile/profile-push-details.schema.json) |
## Schema Hierarchy

* Push Notification Token Details `https://ns.adobe.com/xdm/context/profile-push-details`
  * [Extensibility base schema](../../datatypes/extensible.schema.md) `https://ns.adobe.com/xdm/common/extensible`


## Push Notification Token Details Example
```json
{
  "xdm:pushNotificationTokens": [
    {
      "xdm:token": "ABC123DEFG",
      "xdm:registrationDate": "2017-09-26T15:52:25+00:00",
      "xdm:environment": {
        "xdm:type": "browser",
        "xdm:browserDetails": {
          "xdm:name": "Chrome",
          "xdm:version": "63.0.3239",
          "xdm:acceptLanguage": "en",
          "xdm:cookiesEnabled": true,
          "xdm:javaScriptEnabled": true,
          "xdm:javaScriptVersion": "1.8.5",
          "xdm:javaEnabled": true,
          "xdm:javaVersion": "Java SE 8",
          "xdm:viewportHeight": 600,
          "xdm:viewportWidth": 300
        },
        "xdm:operatingSystem": "iOS",
        "xdm:operatingSystemVersion": "11.2.1",
        "xdm:connectionType": "mobile"
      },
      "xdm:device": {
        "xdm:typeId": "TypeIdentifier-111",
        "xdm:typeIdService": "deviceAtlas",
        "xdm:type": "mobile",
        "xdm:manufacturer": "Apple",
        "xdm:model": "iPhone 6",
        "xdm:modelNumber": "A1586",
        "xdm:screenHeight": 667,
        "xdm:screenWidth": 375,
        "xdm:colorDepth": 16777216
      },
      "xdm:application": {
        "xdm:id": "Abc123",
        "xdm:name": "facebook",
        "xdm:version": "153.0"
      },
      "xdm:channel": {
        "@id": "https://ns.adobe.com/xdm/channels/facebook-feed",
        "@type": "https://ns.adobe.com/xdm/channel-types/social"
      }
    }
  ]
}
```

# Push Notification Token Details Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [xdm:pushNotificationTokens](#xdmpushnotificationtokens) | Push notification token | Optional | Push Notification Token Details (this schema) |
| `*` | any | Additional | this schema *allows* additional properties |

## xdm:pushNotificationTokens
### Push notification tokens

Push notification tokens are used to communicate with applications that are installed on devices or SaaS application accounts.

`xdm:pushNotificationTokens`
* is optional
* type: Push notification token

* defined in this schema

### xdm:pushNotificationTokens Type


Array type: Push notification token

All items must be of the type:
* [Push notification token](../../datatypes/pushnotificationtoken.schema.md) ??? `https://ns.adobe.com/xdm/context/pushnotificationtoken`







