# Contributing

## Getting write access

Open a **Join the Valley** issue on the `.github` repo, or give your GitHub username to a
steward at the venue. Once you're in the `participants` team you can create repos in the
org and transfer your own repos in.

## Bringing a repo in

Two ways, both fine:

- **Transfer** (Settings → Transfer ownership → `valley-of-the-commons`). You keep admin
  on it. Old URLs redirect, so nobody's clone breaks.
- **Create fresh**: `gh repo create valley-of-the-commons/<name> --public --clone`

Keeping it in your own account is also fine — list it on `projects` instead.

## What a repo here needs

1. **A README that works tomorrow.** What it is, who made it, how to run it, what state
   it's in. Half-finished is fine; unexplained is not. Say so plainly if it's a stub.
2. **A license.** Pick one deliberately — the point of this place is that the next hub can
   copy the stack. Common choices here: **AGPL-3.0** or **MIT** for code, **CC BY-SA 4.0**
   for docs and designs, **CERN-OHL-S** for hardware. No license means nobody downstream
   can legally use it.
3. **No secrets.** No `.env`, no keys, no tokens, no `credentials.json`. If one lands in a
   commit, rotate it first and rewrite history second — the rotation is the fix, the
   history rewrite is cosmetics.
4. **Attribution.** If a session produced it, name the people in the README. The P4P
   builds are about keeping a record of who contributed; start with the repo itself.

## Branches

Work on `dev` or a feature branch, merge to `main` when it runs. Nobody is enforcing this —
it's just what keeps a `main` you can hand to someone.

## The Convivial Tool Test

Before adding a dependency, ask the four questions out loud:

- Can anyone here start and stop it without a gatekeeper?
- Does it add a capability, or remove the alternative?
- Could two named people in this room fix or replace it inside a week?
- At what scale does it start costing more than it gives?

Adopt on the first three. Write the fourth answer down as a review trigger.
