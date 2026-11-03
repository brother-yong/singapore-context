# singapore-context

A Claude skill that makes Claude answer like it lives in Singapore, not America.

Without it, Claude tells you to collect payment with Venmo, file taxes with the IRS, and "reach out" with "I hope this finds you well". It calls Muhammad Rizwan bin Hassan "Mr Hassan", which is his father's name. This skill fixes that without being asked.

## What changes

| You ask | Without the skill | With the skill |
|---|---|---|
| How do I collect payment? | Stripe, Venmo, quarterly tax estimates | PayNow QR, UEN, yearly IRAS filing by 18 April |
| Email to Muhammad Rizwan bin Hassan | Dear Mr Hassan | Dear Mr Rizwan |
| Cold-call script for a shop owner | "I wanted to reach out about a game-changer!" | "Hi, is this the owner ah? Quick one." Plus a Do Not Call Registry warning |
| WhatsApp to a colleague | "Hey team! Just a quick heads-up!" | "Meeting shift to Thurs 3pm ah. Same room." |

## What it covers

- **Substance:** CPF not 401(k), PayNow not Venmo, IRAS not IRS, Singpass, ACRA, HDB, MRT, Grab, Shopee, polyclinic, 995 and 999.
- **Formats:** dates (28/7/2026), S$, 8-digit phone numbers, block and unit addresses, metric.
- **Names:** Chinese, Malay, Indian and Sikh naming, so Claude addresses people correctly.
- **Calendar:** public holidays, school terms, NS and reservist duty, no seasons.
- **Legal traps:** Do Not Call Registry, PDPA, Spam Control Act, defamation, advertising rules, race and religion.
- **Wording:** British spelling, local words, office email habits, and which Americanisms to cut.
- **How people talk:** switching between Standard English and Singlish by situation, soft refusals, deflected compliments, Uncle and Auntie, light Singlish grammar, particles and WhatsApp style.

Claude picks the register from the situation. Formal writing stays formal. Sales scripts and WhatsApp get light Singlish. Deep Singlish only appears when you ask for it.

## Install

**Claude.ai or the Claude desktop app**

1. Click the green "Code" button on this page, then "Download ZIP".
2. In Claude, go to Settings > Capabilities > Skills and upload the ZIP.
3. Make sure the skill is switched on.

**Claude Code**

```bash
git clone https://github.com/brother-yong/singapore-context ~/.claude/skills/singapore-context
```

The skill triggers on its own for anything practical. You don't need to mention Singapore or type a command.

## Try it

Start a new chat for each prompt.

- "Write a WhatsApp to my colleague saying the meeting moved to Thursday 3pm."
- "Write the same thing as a formal email to a client."
- "My supplier said 'can try, I see how first'. Are they confirmed?"
- "Write a cold-call script for selling to a hawker uncle."

Then switch the skill off and ask again to see the difference.

## Not legal advice

The legal section flags risks so Claude raises them. It is not legal advice. Rates, limits and deadlines change, so check the official source before relying on a number.

## Licence

MIT. Free to use, change and share.
