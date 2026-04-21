# OpinionGuard — New HVAC Client Onboarding Checklist

Use this checklist every time you onboard a new HVAC client. Load the **OpinionGuard HVAC Client Template v2** snapshot into their sub-account, then complete these steps.

---

## Pre-Setup (Before Loading Snapshot)

- [ ] Create new sub-account in GHL for the client
- [ ] Load **OpinionGuard HVAC Client Template v2** snapshot into the sub-account

---

## Client Information to Collect

Get this from the client before starting setup:

- [ ] Business name (exact as it appears on Google)
- [ ] Owner/manager name and email
- [ ] Phone number for the business
- [ ] Google Business Profile URL
- [ ] Google Review link (get from: Google Maps → their business → "Write a review" → copy URL)
- [ ] Past customer list (CSV with Name, Phone, Email columns)
- [ ] Logo (for branded messages)

---

## Sub-Account Configuration

### Custom Fields
- [ ] Set **Company Name** field → client's business name
- [ ] Set **Google Review Link** field → client's Google review URL

### Phone & SMS
- [ ] Assign a phone number to the sub-account (or port client's number)
- [ ] Register A2P 10DLC brand for the client (if sending SMS)
- [ ] Register A2P campaign

### Email
- [ ] Set up sending domain (or use shared domain)
- [ ] Verify email sender address

---

## Workflow Customization

### 1. Post-Service Review Request
- [ ] Verify survey URL points to this sub-account's survey (not Utmost Inc's)
- [ ] Update company name references in SMS/email templates
- [ ] Test with a sample contact

### 2. Review Rating Router
- [ ] Verify Google Review Link custom value is populated
- [ ] Confirm routing: scores 8-10 → Google, scores 1-7 → private feedback
- [ ] Test the survey → router flow end-to-end

### 3. Review Reactivation Drip
- [ ] Update survey URL in all 3 SMS messages to this sub-account's survey
- [ ] Update survey URL in the follow-up email
- [ ] Verify company name merge field works
- [ ] Test with a sample contact

### Review Rating Survey
- [ ] Confirm survey is active and accessible
- [ ] Note the new survey URL for this sub-account
- [ ] Replace survey URLs in all workflows with the new URL

---

## Go Live

### Past Customer Reactivation
- [ ] Import client's past customer CSV
- [ ] Tag imported contacts with `reactivation`
- [ ] Monitor first 24 hours for any issues or opt-outs

### Ongoing Review Requests
- [ ] Set up trigger for Post-Service Review Request (manual tag, Zapier, or API)
- [ ] Train client on how to trigger review requests after service calls
- [ ] Confirm the full flow works: service complete → tag added → SMS sent → survey → Google review

---

## Post-Launch (First Week)

- [ ] Check review count after 24-48 hours
- [ ] Monitor for any delivery failures or bounces
- [ ] Follow up with client on any negative feedback alerts
- [ ] Confirm team notification is working

---

## Per-Client Customization Reference

| What to Change | Where | Change To |
|---|---|---|
| Survey URL | SMS messages in all 3 workflows + email | This sub-account's survey URL |
| Company Name | Custom field | Client's business name |
| Google Review Link | Custom field | Client's Google review URL |
| Phone number | Sub-account settings | Assigned number |
| Email sender | Sub-account settings | Client's domain or shared |

---

## Notes

- **Survey URL is the #1 thing to update.** Every sub-account gets its own survey URL. If you forget this, reviews will route to the wrong account.
- **Google Review Link** must be the direct review URL, not just the Google Maps listing.
- **A2P registration** can take 1-2 weeks. Plan ahead or use email-only until approved.
- **Reactivation drip** spaces messages out (1hr → 3 days → 5 days → email). Don't rush it.
