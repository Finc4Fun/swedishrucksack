# swedishrucksack.com

Static site for the Swedish M39 Rucksack, hosted on GitHub Pages.

## 1. Fill in the gaps

Search the files for these and replace them:

| Find | Replace with |
|---|---|
| `PAYPAL_M39_LINK` (index.html, 2 places) | Your PayPal payment link for the M39 |
| `PAYPAL_KIT_LINK` (index.html) | Your PayPal link for the conversion kit, then remove `disabled` from that button's class |
| `class="placeholder"` blocks | Text from your old History, Famous M39s, Reviews, FAQ, Terms and Privacy pages |

To get a PayPal link: PayPal Business account → **Pay Links and Buttons** → create a link for the product → copy the URL.

## 2. Add the photos

Save these from the current site (right-click → Save image) into the `images` folder with these names:

| File name | What it is |
|---|---|
| `hero.jpg` | Main product photo of the M39 (also used as the social-share image) |
| `rivets.jpg` | The rivet/conversion kit photo |
| `frameless.jpg` | Photo from the "Going Frameless" blog post |

Add gallery photos as you like and reference them as `images/your-file.jpg`.

## 3. Publish on GitHub

1. Create a new public repository on github.com (e.g. `swedishrucksack`).
2. Upload everything in this folder (**Add file → Upload files**), including `CNAME` and `.nojekyll`.
3. Go to **Settings → Pages**, set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Check the site at `https://<your-username>.github.io/swedishrucksack/` (paths will look right once the custom domain is on).

## 4. Point your domain

At your domain registrar's DNS settings:

- `www` → **CNAME** → `<your-username>.github.io`
- Root (`@`) → **A** records → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`

Then in **Settings → Pages**, enter `www.swedishrucksack.com` as the custom domain and tick **Enforce HTTPS** once it's available (can take up to a day).

Only cancel Weebly after the new site loads at your domain.

## Old links

The old Weebly page addresses (e.g. `/the-m391.html`, `/reviews.html`, `/m39-blog/going-frameless`) redirect to the matching section of the new site, so existing links and bookmarks keep working.
