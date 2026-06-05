# Fake Door Validation Plan — Product #17 Candidate

## Manual Action Required (1 min)

**Enable GitHub Pages:**
1. Open: https://github.com/eylulsenakumral/quarterly-tax-deadline-reminder-fake-door/settings/pages
2. Source: "Deploy from a branch"
3. Branch: `master` / Folder: `/ (root)`
4. Save

**After Pages is live:**
- URL: https://eylulsenakumral.github.io/quarterly-tax-deadline-reminder-fake-door/

## Validation Timeline

### Day 1-2: Traffic + Intent Measurement
- Share to test channels (see copy below)
- Track: visits, signups, CTR

### Day 3: Analysis
- If >5% CTR → Build Product #17
- If <5% CTR → Pivot to Opportunity #2

## Test Channels

### Reddit (if audience matches)
Target subreddits:
- r/freelance
- r/tax
- r/personalfinance
- r/smallbusiness

### LinkedIn
- Freelancer/entrepreneur groups
- Own network

## Analytics Setup

### Option 1: Google Analytics (Free)
Replace line 8 in `index.html`:
```html
<!-- Old -->
<script src="https://cdn.usefathom.com/script.js" data-site="XXXXXX" defer></script>

<!-- New -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### Option 2: Fathom (if account exists)
Replace `XXXXXX` with actual Fathom site ID.

## Success Criteria

| Metric | Target | Decision |
|--------|--------|----------|
| Visits | 100+ | - |
| Signups | 5+ (5% CTR) | ✅ Build |
| Signups | <5% CTR | ❌ Pivot |

## Product #17 (If Valid)

**Quarterly Tax Deadline Reminder**
- Automated reminders for quarterly estimated tax deadlines
- Target: Freelancers, LLCs, S-Corps
- Deadlines: April 15, June 15, Sept 15, Jan 15
- Pricing: $9/mo or $79/year

## Munger's Pre-Mortem (Cycle #318)

1. **Unverified Competition** — QB/Xero/FreshBooks may have this feature
2. **Unverified Channel** — Product #16 channels may not fit this persona
3. **Unverified Willingness to Pay** — "Reminder" may be a commodity

*This 2-day accelerated validation addresses these concerns.*
