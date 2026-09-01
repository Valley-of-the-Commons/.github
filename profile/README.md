# Valley of the Commons

**Popup Village 2026 · 24 August – 20 September · Commons Hub, Reichenau an der Rax, Austria**

[valleyofthecommons.com](https://valleyofthecommons.com) · [commons-hub.at](https://www.commons-hub.at)

This is where code and hardware built at the Valley lives. Four weeks, one anchor
session each weekday, four builds:

| Build | What it answers |
|---|---|
| **Permanent storage node** | Data the valley doesn't rent, doesn't lose, and gets paid to host |
| **Local archive node** | The same knowledge, fast and offline, on a box in this building |
| **P2P wiki as a P4P mesh** | The valley's knowledge over carrier-free radio, with a record of who wrote it |
| **Operational infrastructure** | All of it packaged so the next hub copies it instead of reinventing it |

Everything here is meant to be handed to the Valley e.V. as permanent infrastructure.
If you can't start and stop it without a gatekeeper, it doesn't belong in the valley.

## What's here

| Repo | What it is |
|---|---|
| [**valley-commons-website**](https://github.com/valley-of-the-commons/valley-commons-website) | The site at valleyofthecommons.com — landing page, membership application, sponsorships, and the Socratic game terminal |
| [**commons-spatial**](https://github.com/valley-of-the-commons/commons-spatial) | A laser-scanned building in a browser: 12 KB viewer, no dependencies, in a format any engine can read |
| [**LibreSesh**](https://github.com/valley-of-the-commons/LibreSesh) | A live schedule board for conferences and unconferences. No accounts, no fuss |
| [**mimir**](https://github.com/valley-of-the-commons/mimir) | Facilitation tooling |
| [**holons**](https://github.com/valley-of-the-commons/holons) | — *(needs a README and a description; see house rules)* |
| [**projects**](https://github.com/valley-of-the-commons/projects) | Index of everything built at VOTC26, wherever it's hosted |
| [**project-template**](https://github.com/valley-of-the-commons/project-template) | Starting point for a valley project. Click **Use this template** |
| [**.github**](https://github.com/valley-of-the-commons/.github) | This profile, the contribution guide, and the join-request flow |

Not everything built at the Valley lives in this org, and that's deliberate — the
[`projects`](https://github.com/valley-of-the-commons/projects) index is the complete
picture, including work people keep in their own accounts.

## Put your work here

**You have a repo already** → transfer it: repo → Settings → Transfer → owner `valley-of-the-commons`.
Stars, issues and old URLs come with it.

**You're starting fresh** → click **Use this template** on
[`project-template`](https://github.com/valley-of-the-commons/project-template),
or just `gh repo create valley-of-the-commons/<name> --public`.

**You'd rather keep it in your own account** → fine. Open an *Add a project* issue on
[`projects`](https://github.com/valley-of-the-commons/projects) and it gets listed anyway.
Nothing here requires you to move your work.

## Joining

Open a **Join the Valley** issue on [`.github`](https://github.com/valley-of-the-commons/.github/issues/new/choose).
Any steward in the room approves it with one comment and the invite lands in your inbox.
Or hand your GitHub username to a steward in person — batch invites go out at the end of
each session.

## Who can change what

Being in the org gets you **read** on every repo here, and the ability to create new ones.
It does **not** get you write access to someone else's project. Each repo decides that for
itself.

That's on purpose. A shared village needs everything legible to everyone, and it also needs
the person who built a thing to stay responsible for it. Read-by-default gives you the
first without quietly costing you the second.

**If you maintain a repo and want others pushing to it**, grant it — it takes one action
and it's yours to make:

- **Whole group**: repo → Settings → Collaborators and teams → Add teams → `participants` → **Write**.
- **One person**: same screen, Add people → their username → **Write**.
- **From the CLI**:
  ```
  gh api -X PUT /orgs/valley-of-the-commons/teams/participants/repos/valley-of-the-commons/<repo> -f permission=push
  ```

**If you want to contribute to a repo you can't push to**, fork it and open a pull request,
or ask its maintainer for write. Both are normal. The fork route needs nobody's permission
and is usually faster than waiting for someone to find their laptop.

Stewards approve join requests and curate the index. They are not a gate on your work.

## House rules

Short version: name your license, write a README someone can follow tomorrow, and don't
commit secrets. Longer version in [CONTRIBUTING](https://github.com/valley-of-the-commons/.github/blob/main/CONTRIBUTING.md).

On that third one — if a secret does land in a commit, **rotate it first and rewrite
history second**. The rotation is the fix. The history rewrite is cosmetics, and treating
it as the fix is how a live credential ends up quietly still live.
