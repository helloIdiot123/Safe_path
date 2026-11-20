# Safe Path

A private, one-page guide for people affected by human trafficking in the United States. It has preset questions with plain-language answers, a list of free contacts, a Quick exit button, and a box for typing a question.

The page is a single file (`index.html`) plus three font files in `fonts/`. There is no build step, no database, and no server.

## What the page does with visitor data

- It sets no cookies and has no analytics, ads, or trackers.
- Fonts are served from this site, so a visitor's browser contacts no third party.
- Chosen and typed questions are never sent anywhere. A typed question is matched on the visitor's own device to the closest preset answer.
- Links to other sites do not pass a referrer.
- GitHub Pages keeps ordinary server logs. Do not add analytics to this page.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole page: layout, answers, contacts, and script |
| `fonts/` | Atkinson Hyperlegible and Source Serif 4 (SIL Open Font License) |
| `README.md` | This file |

## Deploy on GitHub Pages

1. Create a public repository, for example `safe-path`.
2. Upload `index.html`, the `fonts` folder, and this README. Keep the folder name and file names exactly as they are.
3. Go to Settings, then Pages. Set Source to "Deploy from a branch", choose `main` and `/ (root)`, and save.
4. After a minute or two the site is live at `https://USERNAME.github.io/REPOSITORY/`.
5. Optional: add a custom domain under Settings, then Pages, create the CNAME record at your domain provider, and tick "Enforce HTTPS".

Before you commit, turn on "Keep my email addresses private" in your GitHub email settings so commits do not show your address.

## Before the public launch

Do each of these and record who did it and when.

- [ ] An anti-trafficking organization or a survivor-informed reviewer has read every answer in `index.html` and approved or changed the wording.
- [ ] Someone with legal knowledge has checked the immigration, police, and records answers for your state or states.
- [ ] Every phone number below has been called or checked on its official site within the last 30 days.
- [ ] The page has been opened on an iPhone, an Android phone, and a desktop browser. Quick exit, Copy buttons, and the chat panel work.
- [ ] A screen reader (VoiceOver or TalkBack) can reach the preset questions and the typing box.
- [ ] The site address uses HTTPS.
- [ ] Someone is named to recheck the numbers every three months and after any news of a hotline change.

## Numbers on the page

All checked against the organization's own website on 12 November 2026, except 911, 988, and 211, which are standard national numbers.

| Contact | Number | Official source |
| --- | --- | --- |
| National Human Trafficking Hotline | 1-888-373-7888, text BEFREE to 233733, live chat | humantraffickinghotline.org |
| National Domestic Violence Hotline | 1-800-799-7233 (800.799.SAFE), text START to 88788 | thehotline.org |
| National Center for Missing & Exploited Children | 1-800-843-5678 (1-800-THE-LOST) | missingkids.org |
| National Runaway Safeline | 1-800-786-2929 (1-800-RUNAWAY) | 1800runaway.org |
| RAINN National Sexual Assault Hotline | 1-800-656-4673 (800.656.HOPE) | rainn.org |
| U.S. Dept. of Labor, Wage and Hour Division | 1-866-487-9243 (1-866-4-USWAGE), weekdays 8:00 to 4:30 local time | dol.gov/agencies/whd |

To change a number, search `index.html` for it. It appears in the `RESOURCES` list and in some of the answers in the `TOPICS` list.

## Editing the answers

Each question is an entry in the `TOPICS` list in the script at the bottom of `index.html`. `q` is the question, `a` is the answer in simple HTML, and `next` names the related questions shown after it. The `KEYS` list controls which preset answer a typed question is matched to.

## Limits

- The page gives general information only. It is not legal, medical, or emergency advice, and it says so.
- It covers the United States. Outside the U.S. visitors are told to call their local emergency number.
- The page cannot close the visitor's browser tab. Quick exit clears the conversation and opens a weather site in a new tab.
- Private browsing does not protect someone whose device has spyware. The page says so.
