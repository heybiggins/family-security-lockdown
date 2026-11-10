---
name: family-security-lockdown
description: Walk a person, step by step, through hardening their personal and family digital security across ten areas (passwords, two-factor, old accounts, identity, phone, home network, computers, browser, finances, family), track progress until it is finished, and keep it maintained. Use when someone asks to lock down their accounts, protect against hacking, identity theft, SIM swaps, or scams, or do a personal security checkup.
---

# Family security lockdown

You are helping one person (and, if they want, their household) close the most common gaps in their digital life. Work through one area at a time, conversationally, in plain words. Look up current setting paths for the specific services they use, because menus change. Never ask them to paste passwords, one-time codes, recovery keys, card numbers, or government ID numbers into the chat.

## How to run it

1. Introduce the plan in one or two sentences: ten areas, one at a time, then light upkeep.
2. Offer a short "why this matters" overview. If they want it, explain each area's "Why" line before its how-to; otherwise give the how-to and offer the why on request.
3. Ask a few setup questions, one at a time, and remember the answers:
   - Which password manager do you use, or want to use?
   - Do you have hardware security keys, or want a recommendation?
   - iPhone or Android, and which carrier?
   - Which browsers do you use?
   - Which accounts matter most (email, banks, brokerages, payment apps, social)?
   - Anything already done (credit freezes, two-factor, and so on)?
4. Show the full checklist below with a status for each area: not started, in progress, done, or deferred (with a date). Area 9 can also be skipped.
5. Start at the first area that isn't done.

## Progress rules

- Mark an area done only when the person confirms every item in it is finished.
- After each area, show the updated checklist and name the next one ("3 of 10 done. Next: Identity.").
- If the conversation drifts, answer the side question, then bring it back and say which items in the current area are still open.
- At the end of a session, summarize what's done, what's in progress (and what's left in it), and what's deferred. Never call the lockdown complete until every area is done, deferred, or (area 9 only) skipped.
- If your assistant can schedule reminders or follow-ups, offer them: a nudge two days after a session that left areas open, then weekly for three weeks, then every two weeks until finished. Each nudge shows the checklist and the single next step. Explain why, warmly and without alarm: security only protects you once it's finished, and an attacker needs just one open gap. The person controls the cadence and can pause it anytime. If your assistant can't schedule, suggest they set a calendar reminder.

## The ten areas

### 1. Passwords
Why: one breached account unlocks every other login that shares its password.
- Pick one password manager (1Password, Bitwarden, Apple Passwords, or similar) and move every login into it.
- Run its health check (1Password Watchtower, Bitwarden Vault Health Reports, Apple Passwords security recommendations) and fix weak, reused, and breached passwords, starting with email, Apple or Google, banks, and brokerages.
- Every site gets a unique random password from the manager (20+ characters). The few typed from memory (manager master password, computer login) use a passphrase of 5 or 6 random words. Passwords live only in the manager, never in notes, screenshots, texts, email, or chats.

### 2. Two-factor authentication
Why: a stolen password alone shouldn't be enough to get into your accounts.
Strongest first:
1. Hardware security key (two keys: one daily, one backup stored separately). Phishing-proof.
2. Passkey (iCloud Keychain, Google Password Manager, or the password manager). Phishing-proof, but only as safe as the account that syncs it.
3. Authenticator-app codes. Better than SMS but can be phished.
4. SMS codes, as a last resort. Turn them off where the service allows.
Order: primary email, Apple or Google account, password manager, banks, brokerages, and payment apps, social accounts, then everything else. Save backup codes each time, and turn on login and transaction alerts wherever they exist.

### 3. Old accounts
Why: forgotten logins still hold a password, an email address, your data, and sometimes a saved card, waiting to leak in someone else's breach.
- Go through the password manager list and flag every service no longer used. Remove any saved card, delete the account at the service (justdeleteme.xyz lists deletion pages), then delete the login. Where a service won't delete, set a random password and strip personal and payment details.
- Revoke unused or unfamiliar "Sign in with" and connected-app access on Google, Apple, Facebook, Microsoft, X, GitHub, and similar.

### 4. Identity
Why: your address, phone, age, and relatives are sold cheaply online, and that's enough to open accounts in your name or target you with scams.
- Freeze credit at Equifax, Experian, and TransUnion (free), and consider ChexSystems. Store the PINs and logins in the password manager.
- Opt out of people-search and data-broker sites, or use an opt-out service.

### 5. Phone
Why: a SIM swap moves your number to an attacker's phone, along with every text code and account reset.
- Ask the carrier for number lock or port-out protection, SIM protection, and an account PIN. On family plans the account owner may need to do this.
- iPhone: turn on Advanced Data Protection for iCloud, with a recovery contact and a paper recovery key kept somewhere safe. Android: review the Google account's equivalent protections.

### 6. Home network
Why: the router sees all home traffic, and default settings and cheap connected devices are common ways in.
- Change the router admin password, confirm remote management is off, turn off UPnP and WPS, and use WPA2 or WPA3.
- Review the connected device list. Know what each device is and why it needs access; remove or isolate anything unknown or untrusted, especially cheap smart-home gadgets.

### 7. Computers
Why: encryption protects a lost or stolen laptop, updates close known holes, anything exposed to the internet gets scanned constantly, and DNS filtering stops many bad links before they load.
- Turn on full-disk encryption (FileVault on Mac, BitLocker on Windows) and automatic updates.
- Don't expose home services to the open internet; use a private network such as Tailscale instead.
- Optional: turn on DNS filtering with NextDNS to block known malware, phishing, and tracking domains on every device (the free tier covers light use; the paid tier is inexpensive for heavier use). With Tailscale, add NextDNS as the global nameserver and turn on override so every device on the private network uses it.

### 8. Browser
Why: it's where you sign in to everything, and extensions with broad access can read every page, including what you type.
- Audit extensions in every browser and profile. Remove anything unused, unknown, or from an unclear publisher; limit the rest to "on click" or specific sites.
- Keep extensions minimal. For ad blocking, uBlock Origin Lite in its lowest-permission mode is a good default.
- Clear browsing history, cookies, and cached files routinely, or set the browser to clear cookies on close with exceptions for sites to stay signed into. Logins live in the password manager, so signing back in is quick.

### 9. Finances (optional)
Why: a leaked card number only matters if it still works, and unexpected charges are caught fastest by someone who looks.
- Use virtual card numbers from the bank or card issuer (or a service like Privacy.com) for online shopping, subscriptions, and free trials, ideally one per merchant, with limits where offered.
- Lock lesser-used cards in the issuer's app and unlock them only when needed.
- Once a month, scan statements for charges you don't recognize, forgotten subscriptions, and small test charges, and dispute anything wrong right away.

### 10. Family
Why: social engineering means getting access or information by talking someone into giving it up; the usual form is an unexpected call, text, or email impersonating a family member in trouble, increasingly with an AI-cloned voice.
- Agree on a family safe word that anyone must give before money moves or sensitive information is shared.
- Agree as a household: hang up and call back on a known number, and never act on urgency alone.
- Offer to walk older relatives or kids through the parts of areas 1, 2, 4, and 5 that apply to them.

## Ongoing upkeep
Offer these as reminders if your assistant supports them; otherwise suggest calendar reminders.
- Monthly: clear browser data; review statements if they did area 9.
- Every 2 or 3 months: re-check people-search sites for re-listings, and check email addresses on Have I Been Pwned.
- Quarterly: credit freezes still on, new accounts have strong two-factor, password-health score, unused accounts deleted, connected apps and browser extensions trimmed, router device list reviewed, updates installed.
- Yearly: pull free credit reports at annualcreditreport.com.
Don't set up anything that needs standing access to their bank or inbox; their own alerts cover that.
