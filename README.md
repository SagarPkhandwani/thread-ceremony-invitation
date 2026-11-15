# Aarav’s Yagyopavit invitation

A Hindi-first, mobile-friendly ceremony invitation inspired by the linked wedding example. It includes an opening invitation card, custom illustration, animated story and ceremony sections, a live countdown, playful blessing interactions, family details, a map link, an RSVP message, and optional music.

This is a static website: no build tools or paid hosting are required.

## Preview on your computer

Open `index.html` in a browser. The Hindi font loads from Google Fonts when you have an internet connection; the rest of the page is included in this folder. The photos/illustration are drawn directly into the site, so there are no required image downloads.

## Personalize the invitation

Open `index.html` in a text editor and use **Find** to replace the sample values below. Replace every occurrence so the welcome card, story, family section, venue and closing message stay consistent.

| Sample text | Replace with |
| --- | --- |
| `आरव` or `आरव शर्मा` | Child’s name |
| `शर्मा परिवार` | Family name |
| `श्री राजेश शर्मा` | Parent/guardian name |
| `श्रीमती नेहा शर्मा` | Parent/guardian name |
| `रविवार` | Correct weekday |
| `17 जनवरी` and `17` | Ceremony date and day number |
| `2027` | Ceremony year |
| `09:30`, `11:30`, `12:30` | Your ceremony, blessing and meal times |
| `द रॉयल आँगन` | Venue name |
| `प्लॉट 24, अशोक विहार, नई दिल्ली — 110052` | Full venue address |
| `नई दिल्ली` | City |

The schedule card copy, family names, and two playful Hindi quote messages are also in `index.html`; edit them there to suit your family. Search for **`एक्स्ट्रा लड्डू`** to find the surprise-message list.

### Update the countdown and links

1. In `script.js`, change `eventAt` to the event date and time in ISO format, including your time-zone offset. Example for India: `new Date('2027-01-17T09:30:00+05:30')`.
2. In `index.html`, update the Google Maps URL next to the venue. You can copy a share link from Google Maps and replace the current `https://maps.google.com/?q=Ashok+Vihar+New+Delhi` address.
3. The final **अपना आशीर्वाद भेजें** button opens WhatsApp with a sample message. Edit its `href` text in `index.html`. To address it to a particular WhatsApp number, use `https://wa.me/COUNTRYCODEPHONENUMBER?text=...` with digits only.
4. To use your own music, put a rights-cleared MP3 at `assets/ceremony-music.mp3`. Visitors start it with the floating music button; it will not autoplay.

## Publish and share with GitHub Pages

1. Create a GitHub repository for the invitation.
2. Upload the contents of this folder to the repository’s top level. Keep `index.html`, `styles.css`, `script.js`, and `assets/` together.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**, then choose the `main` branch and `/ (root)`. Save.
5. Wait for GitHub Pages to finish publishing. Copy the public URL shown in Pages settings and send it to your guests.

Check the published link on a phone before sharing. The invitation is a visual website with links and a copy-address button; it does not collect or store guest RSVPs.
