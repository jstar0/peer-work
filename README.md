# peer-work

An agent skill for working with another model as a peer. Either model can make the first attempt, challenge the framing, or change the work. The skill leaves model choice, timing, and the amount of collaboration open.

For example: “Use peer-work on the landing page. I like the opening scene, but the rest still feels generic.” You can name a peer and a channel if you have a preference. The skill itself is Markdown; it does not launch a service or grant either agent access to another client.

## Install

Clone this repository and copy or symlink the **whole** [`skills/peer-work`](skills/peer-work) folder into a skills directory your client reads. For example, for Claude Code on macOS or Linux:

```sh
git clone https://github.com/jstar0/peer-work.git
mkdir -p ~/.claude/skills
ln -s "$PWD/peer-work/skills/peer-work" ~/.claude/skills/peer-work
```

For Codex, use `${CODEX_HOME:-$HOME/.codex}/skills` as the destination directory. For other clients, use their configured skills directory. Start a fresh session and ask it to use `peer-work`. Symlinked installs follow updates to the checkout.

Read the [skill](skills/peer-work/SKILL.md) for the collaboration guidance and the [client notes](skills/peer-work/references/local-clients.md) for model changes and handoffs.

Released under the [MIT License](LICENSE).
