## Dhruvan Karthik

I build automation and API integration work in Python — the parts that have to
keep running after the demo.

**[automation-demos](https://github.com/hidhruvan-prog/automation-demos)** —
three working automations: document → CRM extraction, a grounded assistant that
refuses to answer off-source, and a lead router with explainable scoring. Zero
credentials, zero network, they run offline in one command each.

I picked those three by surveying 157 automation agencies and counting which
services they actually advertise, then building against the top of the list
instead of guessing.

### What I care about in this work

The AI call is the easy part — anyone can copy it off a docs page. The parts
that decide whether an automation survives contact with production are duller:

- **Explicit failure handling.** Every pipeline needs a visible answer to "what
  happens when it can't?" A review queue, a refusal, a named fallback owner.
- **Idempotency.** Automations get re-run by retries, cron overlaps, and humans
  clicking twice. Run it again; the numbers should not double.
- **Honest reporting.** Successes, failures, and degraded modes counted
  separately. A pipeline printing "6 processed" while one silently vanished is
  how you lose the second job.

The demos README documents the bugs my own sample data caught in my own code,
because finding them is the point.

### Stack

Python · n8n · REST/API integration · SQLite · Claude API · pandas

### Work

Available for contract build work, including white-label under an agency's own
brand. Reach me at hidhruvan@gmail.com.
