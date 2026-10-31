# A Little Love Studio

Static storefront plus seven standalone HTML experiences.

## Run locally
In this folder run `python -m http.server 8000`, then open http://localhost:8000.

## Before accepting orders
Edit `js/main.js` and replace `STORE_CONFIG.whatsappNumber` (`919999999999`) with your WhatsApp Business number in international format, digits only (India example: `919876543210`). The order form deliberately blocks sending while the placeholder remains. The site creates a WhatsApp order enquiry only; it does not take payment or upload photos to a server.

## Personalise templates
Each product HTML has a `const CONFIG` object near the beginning of its script. Edit recipientName, senderName, message, photos, notes, date/occasion and finalMessage where available. Add photo URLs to `CONFIG.photos`; the browser can display local images if you supply data URLs or hosted URLs. The storefront order form previews selected uploads; if WhatsApp does not attach them automatically, send them in the chat.

The project uses plain HTML, CSS and JavaScript and can be hosted on GitHub Pages, Netlify or another static host.
