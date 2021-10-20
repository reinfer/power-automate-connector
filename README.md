A connector for [Re:infer](https://www.reinfer.io) and [Power
Automate](https://flow.microsoft.com/) / [Azure Logic Apps](https://azure.microsoft.com/en-gb/services/logic-apps).

## Background

[Re:infer](https://www.reinfer.io) empowers everyone to create custom
high-quality machine learning models to interpret conversations. No technical
expertise is required with out of the box support for **emails**, **tickets**,
**feedback**, **chat** or **phone calls**.

<p align="center">
 <img src="https://user-images.githubusercontent.com/797170/138135507-d067b0ad-13b5-4384-965d-cc0a55a36265.png" width="544">
</p>

You can use this connector to
 1. import communication data into Re:infer and
 2. perform actions in other systems in response to predictions on new messages

For importing data, you should also consider using Re:infer's native
integrations (e.g. Office 365, Salesforce etc.) as it can be more flexible.

## Get Started

You will need two things

1. A Re:infer account. [Sign up](https://nextcom.no/en/try-the-system-for-free/) for a free trial if you don't have one or [get in touch](support@reinfer.io).
1. An API token for authentication. You can obtain this from your **Manage Account** page.


**IMPORTANT:** When entering the API token in the connector, you need to prefix it with "Bearer" followed by white space, e.g.
```
Bearer REINFER-API-TOKEN
```

_This is unfortunately required because of limitations in the old version of OpenAPI used by Power Automate (v2)._ _

Happy automations!

### Development

To develop the connector, you need a Power Automate account and to install the Python CLI for Power Automate
```
pip install paconn
```

To add the custom connector to your Power Automate account, login and create it with

```
paconn login && paconn create --settings settings.json
```

## Updating the connector


Once created, to update the connector, run
```
paconn update --settings settings.json
```

## Supported Operations
The connector supports the following operations:

TODO: fill in all the supported operations

## Resources
You can find our API documentation and developer docs [here](https://developers.reinfer.io).

For any questions, please feel free to [contact us](support@reinfer.io).
