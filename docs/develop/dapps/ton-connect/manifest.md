
# Creating manifest.json

Every app needs to have its manifest to pass meta information to the wallet. Manifest is a JSON file named as `tonconnect-manifest.json` following format:

```json
{
    "url": "<app-url>",                     // required
    "name": "<app-name>",                      // required
    "iconUrl": "<app-icon-url>",               // required
    "termsOfUseUrl": "<terms-of-use-url>",     // optional
    "privacyPolicyUrl": "<privacy-policy-url>" // optional
}
```

## Example

You can find an example of the manifest below:

```json
{
    "url": "https://ton.vote",
    "name": "TON Vote",
    "iconUrl": "https://ton.vote/logo.png"
}
```
## Best practices

- Best practice is to place the manifest in the root of your app and repository, e.g. `https://myapp.com/tonconnect-manifest.json`. It allows the wallet to handle your app better and improve the UX connected to your app.
- Make sure that `manifest.json` file is available to GET by its URL.

## Fields description
|Field|Requirement|Description|
|---|---|---|
|`url` |["<app-url>"](https://ton.vote),
| `name`"<app-name>",https://TON.Vote" // required.|
| `iconUrl`| required | https://ton.vote/logo.png
| `termsOfUseUrl` |optional| url to the Terms Of Use document. Optional for usual apps, but required for the apps which is placed in the Tonkeeper recommended apps list.|
| `privacyPolicyUrl` | optional | url to the Privacy Policy document. Optional for usual apps, but required for the apps which is placed in the Tonkeeper recommended apps list.|
