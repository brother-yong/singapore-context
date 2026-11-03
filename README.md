# singapore-context

A Claude skill that makes Claude default to Singapore instead of America.

Ask Claude how to collect payment and it says Stripe and Venmo. Ask it to draft an email and it writes "reach out" and "I hope this finds you well". Ask it to address Muhammad Rizwan bin Hassan and it writes "Dear Mr Hassan". This skill fixes that, silently.

## What it covers

- **Substance:** CPF not 401(k), PayNow not Venmo, IRAS not IRS, Singpass, ACRA, HDB, MRT, Grab, Shopee, polyclinic, 995/999.
- **Formats:** dates (28/7/2026), S$, 8-digit phone numbers, block and unit addresses, metric.
- **Names:** Chinese, Malay, Indian and Sikh naming, so Claude addresses people correctly.
- **Calendar:** local public holidays, school terms, NS and ICT, no seasons.
- **Legal traps:** Do Not Call Registry, PDPA, Spam Control Act, defamation, advertising rules, race and religion.
- **Wording:** British spelling, Singapore English, which Americanisms to cut, and when light Singlish fits (sales calls, scripts) and when it doesn't (formal writing).

## Install

Claude Code:

```bash
git clone https://github.com/brother-yong/singapore-context ~/.claude/skills/singapore-context
```

Claude.ai or Claude Desktop: download this repo as a ZIP and upload it under Settings > Capabilities > Skills.

It triggers on its own for anything practical. No command needed.

## Not legal advice

The legal section flags risks so Claude raises them. It is not legal advice. Rates, limits and deadlines change, so check the source before relying on a number.

## Licence

MIT. Made by Tan Yong Han, Singapore.
