# Domain Email Plan

## Recommended addresses

| Address | Purpose |
|---|---|
| hello@sendwaste.ai | General enquiries |
| founders@sendwaste.ai | Founder correspondence |
| pilots@sendwaste.ai | Pilot customers and onboarding |
| partnerships@sendwaste.ai | Brands, institutions, funders and technical partners |
| support@sendwaste.ai | Product and operational support |
| security@sendwaste.ai | Security reports |
| privacy@sendwaste.ai | Privacy requests |
| finance@sendwaste.ai | Billing and settlement administration |

## Fastest low-cost setup

### Option A: Cloudflare Email Routing

Use free inbound aliases that forward to existing Gmail addresses. This is suitable for immediate verification emails and cloud-credit applications. It does not provide a native outbound mailbox by itself.

### Option B: Zoho Mail or Google Workspace

Use a hosted mailbox for reliable sending and receiving from the domain. Configure SPF, DKIM and DMARC before external applications.

## Required DNS controls

- MX records from the selected mail provider;
- SPF record authorising approved senders;
- DKIM signing key;
- DMARC policy starting with monitoring, then moving to enforcement;
- a dedicated security contact;
- no shared passwords.

## Suggested first aliases

Start with:

- `hello@sendwaste.ai` -> Bethel and the Admin Officer;
- `partnerships@sendwaste.ai` -> CEO and CTO;
- `pilots@sendwaste.ai` -> Hub Manager, CEO and CTO;
- `security@sendwaste.ai` -> CTO;
- `privacy@sendwaste.ai` -> CTO and Admin Officer.
