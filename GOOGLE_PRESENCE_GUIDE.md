# Google Search & Local Presence Playbook
## Singh Billiards & Sports, Jaipur

This guide outlines the precise steps needed to claim, secure, and grow the Google presence of **Singh Billiards & Sports**. We have already pre-installed all necessary SEO code on the website. Follow these simple steps to activate them.

---

## 1. Google Search Console Setup (Crawler Control)
Google Search Console is a free service that allows you to submit your site directly to Google, monitor crawl health, and see search keywords.

### How to Get Indexed:
1. Go to [Google Search Console](https://search.google.com/search-console).
2. Log in using your primary business Google/Gmail account.
3. Click **Add Property** and select **URL Prefix**.
4. Enter your production website URL (e.g., `https://singhbilliards.com/`).
5. Choose **HTML Meta Tag** as the verification method.
6. Copy the code provided by Google (it looks like `google-site-verification=xxxxxxxxx...`).
7. Open [index.html](file:///c:/singh%20billiards/index.html) and locate line 19:
   ```html
   <meta name="google-site-verification" content="PLACEHOLDER_FOR_YOUR_GOOGLE_VERIFICATION_CODE" />
   ```
8. Replace `PLACEHOLDER_FOR_YOUR_GOOGLE_VERIFICATION_CODE` with your code, save, and publish.
9. Click **Verify** in Google Search Console.

### How to Submit the Sitemap:
1. In Search Console, click on **Sitemaps** in the left-hand navigation pane.
2. Under "Add a new sitemap", type `sitemap.xml` and click **Submit**.
3. Google will now automatically scan all your pages, including your high-quality product catalog PDF, ensuring they are beautifully displayed on Google Search.

---

## 2. Google Analytics (GA4) Activation
We have pre-wired the official Google Global Site Tag (`gtag.js`) template inside the `<head>` of your `index.html` file.

### How to Activate Tracking:
1. Visit [Google Analytics](https://analytics.google.com/).
2. Create a new account and set up a **Google Analytics 4 (GA4)** property for your website.
3. Obtain your **Measurement ID** (which will look like `G-XXXXXXXXXX`).
4. Open [index.html](file:///c:/singh%20billiards/index.html) and locate lines 21 to 30:
   ```html
   <!-- 
   <script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
   <script>
     window.dataLayer = window.dataLayer || [];
     function gtag(){dataLayer.push(arguments);}
     gtag('js', new Date());
     gtag('config', 'G-XXXXXXXXXX');
   </script>
   -->
   ```
5. Remove the HTML comments (`<!--` and `-->`) around the tag.
6. Replace both occurrences of `G-XXXXXXXXXX` with your actual **Measurement ID** (e.g., `G-1A2B3C4D5E`).
7. Save and publish. You will now track all visitor traffic, page-views, and clicks!

---

## 3. Google Business Profile & Google Maps (Local SEO)
Because Singh Billiards has a physical display room in Raja Park, Jaipur, local SEO is **extremely powerful**. Most high-intent customers search for *"Snooker table manufacturer Jaipur"* or *"buy pool table near me"* on Google Maps.

### How to Claim & Optimize Your Maps Location:
1. Visit [Google Business Profile](https://www.google.com/business/).
2. Log in and search for **Singh Billiards & Sports, Jaipur** (or create a new profile if it doesn't exist).
3. Ensure the address and details match your website exactly:
   * **Name:** `Singh Billiards & Sports`
   * **Address:** `3/341, LBS College Marg, Raja Park, Jaipur, Rajasthan – 302004`
   * **Phone:** `+91 82099 80262`
   * **Website URL:** `https://singhbilliards.com/` (Make sure this matches your final domain).
   * **Primary Category:** `Sporting Goods Store` or `Billiards Supply Store`.
4. **Opening Hours:** Monday to Saturday (10:00 AM – 7:00 PM), Sunday (By Appointment).
5. **Upload Brand Photos:** Upload high-resolution photos of your snooker tables, pool tables, foosball tables, display room, and your logo (`images/logo.png`).
6. **Encourage Reviews:** Share your Google review link with past clients. 5-star ratings will boost your ranking in the "Local 3-Pack" (the top three local listings displayed on regular Google search results).

---

## 4. Why the New Metadata Matters

* **Local Schema Markup (JSON-LD):** Search engines read the script we added to the head of `index.html`. It explicitly tells Google the exact latitude and longitude of your business, which helps Google show your website when users near Raja Park search for pool/snooker tables.
* **Open Graph Preview:** When you or a client shares `https://singhbilliards.com/` on WhatsApp, it will generate a rich preview card with the Singh Billiards logo, a luxurious title, and a professional description, rather than just showing a raw web link.
* **Search Compliance (robots.txt & sitemap.xml):** Google's search crawlers will locate `robots.txt` immediately upon arriving at your site, find the `sitemap.xml`, and index the site structure efficiently.
