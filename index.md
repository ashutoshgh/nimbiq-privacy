# Nimbiq — Privacy Policy

_Effective date: 14 October 2026 · Last updated: 14 October 2026_

This policy explains what information the Nimbiq weather app ("Nimbiq", "the app") uses,
why, who receives it, how long it is kept and what rights you have. It applies to the
Android app and to the online services it relies on. It is written to meet the EU and UK
General Data Protection Regulation (GDPR), US federal and state privacy laws (including the
California Online Privacy Protection Act and the California Consumer Privacy Act as amended),
the US Children's Online Privacy Protection Act, and India's Digital Personal Data
Protection Act, 2023.

**In short:** Nimbiq has no accounts, no ads, no analytics and no tracking. It uses a
location — either your device's approximate location, if you allow it, or a city you
search for — only to fetch weather for that place. We do not sell or share your
information for advertising, and nothing we store is linked to you or your device.

## 1. Who is responsible

Nimbiq is developed and published by **Ashutosh Ghodasara**, an individual developer
based in India ("we", "us", "our"). For the purposes of the GDPR, we are the controller
of the personal data described here.

**Contact:** a dedicated privacy email address is being set up and will be listed here.
Until then, you can reach us by opening an issue at
[github.com/ashutoshgh/nimbiq-privacy/issues](https://github.com/ashutoshgh/nimbiq-privacy/issues).
Issues are public, so please do not include personal details in one; we will reply with a
private way to continue.

## 2. Information we process

| Information | Where it comes from | Required? |
|---|---|---|
| **Approximate location** (coordinates) | Your device's coarse location, only if you choose "Use current location" and grant permission | No — you can search for a city instead |
| **Coordinates of places you save or search for** | The place you pick from search | Yes, to show weather for that place |
| **The text you type into place search** | You | Only when you search |
| **IP address and basic connection data** (such as the time of the request) | Sent automatically whenever any app connects to the internet | Yes, technically necessary to deliver data to your device |
| **Your OpenWeatherMap API key** | You, only if you choose OpenWeatherMap as the provider | No |
| **Crash reports** | Google Play, only if you have allowed your device to share usage and diagnostics with Google | No |

The app only ever requests **approximate (coarse) location**, never precise location. It
does not request background location access, so Android does not let it read your location
while you are not using it; background updates for widgets and notifications use your
saved places. It does not collect your name, email address,
phone number, contacts, photos, files, device identifiers, advertising ID or any
information about other apps you use.

## 3. How we use it and our legal bases

| Purpose | Information used | Legal basis (GDPR) |
|---|---|---|
| Show forecasts, air quality, pollen, rain alerts and "compared to normal" for the places you choose | Coordinates, search text, IP address | Providing the service you request (Art. 6(1)(b)) |
| Read your device's location when you ask for it | Approximate location | Your consent, given through Android's permission prompt (Art. 6(1)(a); EU ePrivacy rules). You can withdraw it at any time in Android settings |
| Show official weather and disaster warnings for your places | Coordinates | Providing the service you request (Art. 6(1)(b)) |
| Keep the service fast, reliable and within its free data quotas: a short-lived shared weather cache and an anonymous log of which map areas were requested | Coordinates rounded to a grid (see section 5) | Our legitimate interest in running a reliable service at low cost (Art. 6(1)(f)) |
| Notifications (rain, severe weather, daily briefing) | Weather data for your saved places, processed on your device | Your choice to turn them on in Settings; all are off by default |
| Use OpenWeatherMap as your forecast provider | Coordinates and your API key | Providing the service you request (Art. 6(1)(b)) |

We do not use your information for advertising, profiling or any automated decision that
has legal or similarly significant effects on you.

## 4. Who receives your information

Your information is sent over encrypted (HTTPS) connections only to the services needed to
answer your request:

| Recipient | What it receives | Why |
|---|---|---|
| Nimbiq weather service, hosted by Supabase in the EU (Paris) | Coordinates, IP address | Fetches forecasts and air quality from Open-Meteo and caches them; looks up official alerts for India and Europe; works out the usual weather for the date ("compared to normal") |
| Open-Meteo (open-meteo.com) | Coordinates, IP address | Weather, air-quality and historical climate data; the app also contacts it directly if our service is unavailable |
| OpenStreetMap Foundation, Nominatim (UK) | Coordinates, IP address | Turns your device's location into a place name |
| Open-Meteo Geocoding | Your search text, IP address | Place search |
| US National Weather Service (weather.gov) | Coordinates and IP address, only for places in the United States | Official US weather alerts |
| OpenWeather Ltd (UK), only if you enable it with your own API key | Coordinates, your API key, IP address | Alternative forecast provider |
| Google (Google Play) | Crash reports, if your device shares diagnostics | App stability |

Official warnings for India come from NDMA SACHET and for Europe from MeteoAlarm; our
service downloads their public feeds and matches them to your place, so your location is
not sent to them. Global disaster alerts come from GDACS (gdacs.org) as a single global
feed; your location is not sent to GDACS.

Each of these services handles the data under its own privacy policy, for example
[Supabase](https://supabase.com/privacy), [Open-Meteo](https://open-meteo.com/en/terms),
[OpenStreetMap Foundation](https://osmfoundation.org/wiki/Privacy_Policy),
[OpenWeather](https://openweather.co.uk/privacy-policy) and
[Google](https://policies.google.com/privacy).

We do not sell your personal information, "share" it for cross-context behavioural
advertising (as defined by California law), or disclose it to anyone else, except where
the law requires us to.

## 5. How long information is kept

| Information | Where | How long |
|---|---|---|
| Saved places, settings, cached forecasts, your OpenWeatherMap key | Only on your device | Until you delete them or clear the app's storage |
| Shared weather cache (coordinates rounded to about 5 km) | Our service | Refreshed every 15 minutes, deleted within a day |
| Anonymous log of requested map areas (about 5 km squares and the time) | Our service | 30 days, then deleted automatically |
| "Compared to normal" averages (for squares of about 25 km) | Our service | Kept, because they describe the climate of an area and are shared by everyone in it; they contain nothing about you |
| Work queue for areas whose averages are still being calculated | Our service | Until the calculation finishes, usually minutes and at most a few days |
| Network logs, including IP addresses | Our hosting provider (Supabase) and the providers above | Under their own policies; we do not copy or keep them |

None of the records we store contains an identifier that links them to you or your device.

## 6. Data on your device and backups

Your OpenWeatherMap API key is stored encrypted and is never included in backups. If
Android backup is turned on for your device, your saved places and settings may be
included in your Google account backup so they can be restored to a new phone; this is
controlled by your device settings and Google's terms, not by us.

## 7. International transfers

Our service is hosted in the EU. Some recipients listed in section 4 are in other
countries, including the United Kingdom and the United States, and we are based in India.
Where the GDPR applies, transfers outside the EU/EEA rely on an adequacy decision (for
example for the United Kingdom, Switzerland and US companies certified under the EU–US
Data Privacy Framework), on the recipient's standard contractual clauses, or on being
necessary to provide the service you asked for (Art. 49(1)(b)), such as fetching US
alerts for a place in the US.

## 8. Your rights

**Everyone.** You can use Nimbiq without granting location access, revoke location access
at any time in Android settings, turn notifications off in the app, and remove all data the
app stores on your device by deleting your places or clearing the app's storage in Android
settings. There is no account to delete.

**EU, EEA and UK (GDPR).** You have the right to access, rectify or erase your personal
data, to restrict or object to its processing (including processing based on our
legitimate interests), to data portability, and to withdraw consent at any time without
affecting earlier processing. You also have the right to lodge a complaint with a data
protection supervisory authority, in particular in the country where you live or work.
Because the records we keep are not linked to you or your device, we usually cannot
identify any data as yours (Art. 11 GDPR); if you can give us details that let us do so,
we will act on your request.

**United States.** We do not sell personal information, share it for targeted advertising,
or use it for profiling. We do not collect precise geolocation or other "sensitive personal
information". Residents of California, Virginia, Colorado, Connecticut, Utah, Texas, Oregon
and other states with privacy laws may request access to, correction of or deletion of
their personal information, and we will not discriminate against anyone for exercising
these rights. Because we do not sell or share personal information, there is nothing to
opt out of, and opt-out preference signals such as Global Privacy Control do not change how
the app behaves. **Do Not Track:** the app does not track you across apps or websites, so
it responds to Do Not Track signals the same way it treats everyone.

**India (DPDP Act, 2023).** You may request a summary of your personal data and how it is
processed, its correction or erasure, and you may nominate another person to exercise
these rights for you. Grievances can be sent to us using the contact in section 1; we aim
to respond within 30 days. You may also approach the Data Protection Board of India.

To make any request, use the contact in section 1. We will respond within the time the
applicable law requires (for example one month under the GDPR, 45 days under California
law), and we may need to ask for information to confirm the request is yours.

## 9. Children

Nimbiq is a general-audience weather app and is not directed at children under 13 (or the
minimum age for consent in your country, such as 16 in parts of the EU). We do not
knowingly collect personal information from children. If you believe a child has provided
us with personal information, contact us and we will delete it.

## 10. Security

All connections use HTTPS. Our database is not publicly accessible, stores only rounded
coordinates and weather data, and is reachable only by our own service. Your OpenWeatherMap
key is encrypted on your device. No system is perfectly secure, but we keep the information
we hold to the minimum the app needs.

## 11. This page

This policy is hosted on GitHub Pages. GitHub may record technical data such as your IP
address when you visit it, under the
[GitHub Privacy Statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement).

## 12. Changes to this policy

If we change this policy, we will post the new version at this address and update the
dates at the top. If a change materially affects how your information is used, we will
also mention it in the app's release notes before it takes effect.

## 13. Contact

Ashutosh Ghodasara, developer of Nimbiq. See section 1 for how to reach us.
