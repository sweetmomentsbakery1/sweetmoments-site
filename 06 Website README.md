# TASK 6 — THE WEBSITE: FILES, PROMPTS, ADDRESS AND TEST RESULTS
### Topic 7 · Web Builders: Mbaziira Simon · Biraro Apollo (backup) · Checked by: Niragire Esther

**Hand-in:** the live web address, screenshots on a phone and on a computer, and the prompts you used.

---

## 1. Every file in the folder, and what it does (be ready to explain this)

```
sweetmoments-site/
├── index.html        Home: heading, one sentence about us, "Order on WhatsApp" button, three reasons to choose us
├── products.html     All ten products with name, description, price in UGX, picture and a filter by collection
├── about.html        Our story, our values, and the ten-member team with their roles
├── pay.html          How to Pay and Order: 5 methods × (3 steps + details), confirmation, refunds, delivery fees
├── policies.html     Delivery, returns, privacy notice (Data Protection and Privacy Act, 2019), short terms, claims table
├── style.css         ALL the design for every page — colours, fonts, layout, menu, cards, footer, phone sizes
├── logo.svg          The round cupcake logo, also used as the browser tab icon (favicon)
├── README.md         This file: the explanation, prompts, test results and publishing steps
└── images/
    ├── hero.jpg          The big background picture on the home and inner pages
    ├── about.jpg         Piping a cake — used on the home page and the About page
    ├── process.jpg       A baker with fresh rolls — About page
    ├── product1..product8.jpg   The eight product photos, named in the order the site expects
```

**How the files work together, in simple words:**
`index.html`, `products.html`, `about.html`, `pay.html` and `policies.html` are five pages of text. Each one starts with `<link rel="stylesheet" href="style.css">`, so all five share one design file — change a colour once in `style.css` and all five pages change. The pictures live in `images/` and are called by file name (`images/product1.jpg`); if a name or the folder name is wrong, the picture shows as a broken icon. The menu and the footer are copied into all five pages so they never disagree. Everything is **HTML + CSS only — there is no JavaScript in this site at all.**

**Why the mobile menu works without JavaScript:** a hidden checkbox (`#nav-toggle`) sits next to the ☰ label; ticking it with `:checked ~ .nav` slides the menu open. The category filter on `products.html` works the same way with radio buttons.

---

## 2. The web address we chose, and why

| Field | Address |
|---|---|
| **Free address (live now)** | `https://sweetmomentsbakery1.github.io/sweetmoments-site/` — GitHub Pages gives https (padlock) for free on public repositories. |
| **The address the business would buy** | **`www.sweetmoments.co.ug`** |

**Why `sweetmoments.co.ug`:**
1. **`.co.ug` says "Uganda"** — a customer in Kitintale trusts a local ending more than a `.com` owned by someone abroad, and it matches our Google profile area.
2. **It is short and easy to say out loud** on the phone: *"go to sweet moments dot co dot ug"* — no hyphens, no numbers, easy to spell after hearing it once.
3. **It matches the brand everywhere** — the same words appear on the sign, the WhatsApp catalogue, the Facebook page and the email signature, so customers never have to guess.
4. **It is a business ending, not a personal one** (`.co.ug` for commerce), which suits a shop that also sells wholesale to cafés, schools and offices.

---

## 3. The prompt used (Appendix A, filled in)

```
I am a student with no coding experience. Please build a simple website for the business
below, using only HTML and CSS. Explain things in simple words.

ABOUT THE BUSINESS
Name: Sweet Moments Bakery
What it sells: bread, cookies, cupcakes, birthday cakes, pastries and muffins; also
  wholesale trays for cafés, schools and offices
Customers: everyday households in Kampala, plus cafés, schools, offices and event planners
Place and delivery area: Kitintale, Nakawa, Kampala — delivers to Kitintale, Ntinda,
  Namuwongo, Nakawa, CBD, Bukoto, Kisaasi, Kololo
Style in three words: warm, friendly, reliable
Colours: main #6F3B1E (cocoa brown), second #E9A33A (golden caramel), background #FFF9F2 (cream)
Contact: WhatsApp +256 750 568 522, email sweetbakeries@gmail.com,
  hours Mon–Fri 6am–8pm, Sat 6am–9pm, Sun 7am–6pm
One sentence about why customers should choose us: We bake everything from scratch every
  morning in Kitintale and deliver it anywhere in Kampala the same day, at published prices.

PAGES I NEED (five pages)
1. index.html: Home, with a big heading, one sentence about us, a button that says
   Order on WhatsApp, and three reasons to choose us.
2. products.html: at least six products, each with a name, a short description, a price
   in UGX and a picture.
3. about.html: our story and our values.
4. pay.html: How to Pay and Order. Show these payment methods, each in its own box with
   three simple steps and the details to pay to: MTN Mobile Money, Airtel Money, bank
   transfer for business customers, cash on delivery in named areas, and card payment
   through a payment provider. Use clearly marked SAMPLE numbers. Add a note that says:
   This is a student project, payments are not active. Also explain how we confirm a
   payment, and our refund rule.
5. policies.html: delivery, returns, a short privacy notice and short terms.
A file called style.css should hold all the design for every page.

RULES FOR THE WEBSITE
Make it look good on a phone first. Use the same menu and footer on every page.
The footer must say: Student project for BUC3106 at MUBS.
Do not invent real phone numbers, prices, awards or customer reviews. Mark any example as SAMPLE.
Use simple picture names, such as hero.jpg, product1.jpg, product2.jpg, and put them in a
  folder called images.
Write short comments in the code that explain each part in plain English.
```

**Follow-up prompts used (Appendix B):**

| # | Prompt (short) | What changed |
|---|---|---|
| 1 | *"Make the Products page filter itself by collection using only CSS radio buttons — no JavaScript."* | Added the `.catalog` filter block to `style.css`. |
| 2 | *"Add a mobile menu that opens when the ☰ label is tapped, still no JavaScript."* | Added `#nav-toggle` + `:checked ~ .nav` rules. |
| 3 | *"Add the SAMPLE student-project banner to the top of every page and the disclaimer to the footer."* | `.topbar` strip and the two footer lines. |
| 4 | *"My website shows plain black text on white and the pictures are missing — explain why."* | Cause: `style.css` and `images/` were not next to `index.html`. Fixed by moving them into one folder (this is exactly Step 6 of Part 6). |
| 5 | *"Make the prices table readable on a small phone."* | Added `.table-wrap { overflow-x:auto }` and larger padding. |

---

## 4. How to test it on your computer (Part 6, Step 6)

1. Put **all** page files, `style.css`, `logo.svg` and the `images/` folder in **one** folder (`sweetmoments-site`).
2. Turn on file name extensions (File Explorer → View → Show → File name extensions) so you can see `index.html` and not `index.html.txt`.
3. Double-click `index.html` — it opens in the browser.
4. Click **every** menu link on **every** page. Check: colours appear (if not, `style.css` is missing or misspelled), pictures appear (if not, check `images/` and the exact file name), and the page stays readable at 390 px width (drag the window narrow).
5. Test that the ☰ menu opens on a narrow window and that the product filters hide/show the right cards.

---

## 5. Publishing with GitHub Pages (Part 6, Step 8)

1. Sign in to github.com with the **group email** → **+** → *New repository* → name it `sweetmoments-site` → **Public** → Create repository.
2. **Add file → Upload files** → drag the *contents* of the folder (the five `.html` files, `style.css`, `logo.svg`, `README.md` and the `images` folder) — **not** the outer folder, so `index.html` sits at the top.
3. **Commit changes.**
4. **Settings → Pages** → Source: *Deploy from a branch* → branch **main**, folder **/ (root)** → **Save**.
5. Wait 2–3 minutes and refresh: the message shows your live address (`https://…github.io/sweetmoments-site/`). Open it on a phone — it starts with **https** and shows a padlock.
6. **Settings → Collaborators** → invite every group member, so their changes carry their names.

---

## 6. Reality check — five people who had not seen the site

*Rule: write down what really happened, then fix at least three problems.*

| Tester | Task given | Where they got stuck | Fix we made | Re-tested? |
|---|---|---|---|---|
| 1 ______ | Find the price of a product | | | ☐ |
| 2 ______ | Find how to pay | | | ☐ |
| 3 ______ | Find the delivery information | | | ☐ |
| 4 ______ | Order on WhatsApp in one tap | | | ☐ |
| 5 ______ | Find a birthday cake on a phone | | | ☐ |

**Three problems we already found and fixed during the build:**

1. **Prices were only in pictures.** → Fixed: added a full HTML price table (`products.html`, "One table, every price") that anyone can read or search.
2. **The mobile menu button overlapped the logo on small phones.** → Fixed: `margin-left:auto` on the label and a 44 × 44 px tap target.
3. **Payment numbers looked real.** → Fixed: every bank/mobile-money figure now carries a red **SAMPLE** badge and the page opens with "Payments are not active".
4. *(Add the three problems your testers find here.)*

---

## 7. Screenshots to collect

- **Computer:** home page, products page with a filter ticked, How to Pay page, Policies page (1440 px wide)
- **Phone:** home page, products page, How to Pay page (390 × 844)
- **Evidence file names:** `site-desktop-home.png`, `site-desktop-products.png`, `site-desktop-pay.png`, `site-phone-home.png`, `site-phone-pay.png`, `site-phone-policies.png`

---
*Prepared for BUC3106 E-Commerce Capstone Project.*
