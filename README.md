# CBot.Modules

An collection of open source modules written for [SreBot](https://github.com/AshleyPoole/srebot) against the [CBot framework](https://github.com/AshleyPoole/CBot).

<br>

## Incident Module

Adds ability to manage incidents and keeps track of status including postmortem links.

### Example Command(s)

`@bot new incident The web server is offline`

### Configuration

Example bot configuration:

```json
    "IncidentManagement": {
		"IncidentNotificationChannel": "incidents",
		"PostmortemTemplateLink": "http://mywebsite/postmortem-template",
		"Warrooms": "incident-warroom0,incident-warroom1,incident-warroom2",
		"AzureConnectionString": "DefaultEndpointsProtocol=https;AccountName=YOUR_ACCOUNT_NAME;AccountKey=YOUR_ACCOUNT_KEY;
	}
```

<br>

## Cloudflare Module

Allows purging of Cloudflare cache for a given zone or a particular cache tag within a zone.

### Example Command(s)

`@bot purge cloudflare zone ashleypoole.co.uk`

### Configuration

```json
"Cloudflare": {
		"AuthEmail": "YOUR_EMAIL_ADDRESS",
		"AuthKey": "YOUR_CLOUDFLARE_AUTH_KEY",
		"ApiUrl": "https://api.cloudflare.com/client/v4"
	}
```
