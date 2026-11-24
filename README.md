# AI asks. You decide.

> *AI can generate OK code. You can generate GOAT decisions.*

A free Claude skill for developers who keep planning but never start.

It doesn't write your plan for you. It asks questions, digs into *why*, and pushes back (always with a reason), while **you make every decision about your product**. You leave with a short product brief in your own words and **one small move for tomorrow**.

Created by **Patricija · [CodeCoffeeChaos](https://instagram.com/codecoffeechaos)**.

---

## Who it's for

You're a developer or technical founder. You're tired of your job and want to build your own thing, but you haven't started yet. There's always one more course, one more podcast, the perfect stack, AI integration, dark mode, the right domain name…

You don't need more information. You need clarity and a first step.

## What you get

One conversation, step by step:

1. **Where are you?** What you want to build and what's stopped you so far.
2. **Why you.** What got you into this idea.
3. **Who it's for.** One specific person and their problem.
4. **One-line promise.** `[Product]: [what the user does] so they can [what they get].`
5. **Core loop.** The one thing your user does again and again.
6. **Signature mechanic** (optional). What makes it feel different.
7. **Your 3 biggest decisions** and the "because…" behind each.
8. **Later, not now.** Things you want someday, but not in the first version of your app. Writing them down stops them from blocking you.
9. **One move for tomorrow.** Small enough that there's no excuse.

At the end you get a markdown brief ready to paste into Notion, Obsidian or a README. See [`examples/example-brief.md`](examples/example-brief.md).

## How it works

- **You go first.** It asks what's already in your head before it suggests anything.
- **One decision at a time,** usually one question at a time.
- **Every pushback has a reason:** your own words, your research, a named principle (Rule of One, the stranger test, counting the cost) or an honest "my gut feeling". No made-up stats.
- **No verdicts.** It never says "this is the best idea". If your reason holds up, it drops the point.
- **Its ideas come after yours,** max 3, marked 🟡 *raw material, reject freely*.
- **Say "no, I'm going with it"** to close any topic.
- **Stack talk waits.** Frameworks, AI features and domain names go on the "Later, not now" list until the person and the problem are clear.
- It speaks English by default and switches if you write in another language.

## Install

### Claude app (web, desktop, mobile)

1. Download [`dist/ai-asks-you-decide.zip`](dist/ai-asks-you-decide.zip). Don't unzip it.
2. In Claude, go to **Customize → Skills**, click **+**, then **Create skill → Upload a skill**, and pick the zip.
3. Make sure **Code execution and file creation** is turned on in your settings. Skills need it.

### Claude Code

```bash
git clone https://github.com/Patusznik/ai-asks-you-decide.git
mkdir -p ~/.claude/skills
cp -r ai-asks-you-decide/ai-asks-you-decide ~/.claude/skills/
```

## Use it

Start a new chat and type:

```
/ai-asks-you-decide
```

or just say something like *"I keep planning my app but never start. Help me get clear."*

Plan for 30–60 minutes. You don't have to finish in one go. Come back with your half-done brief and it picks up where you stopped.

## Stuck on the non-technical side?

Who it's for, positioning, how to tell people about it: I do 1:1 product strategy consultations for developers → **[codecoffeechaos.cyberspell.tech](https://codecoffeechaos.cyberspell.tech)**

Follow along on Instagram: [@codecoffeechaos](https://instagram.com/codecoffeechaos)

## Repo structure

```
ai-asks-you-decide/
├── ai-asks-you-decide/
│   └── SKILL.md          # the skill itself
├── dist/
│   └── ai-asks-you-decide.zip   # ready to upload to the Claude app
├── examples/
│   └── example-brief.md  # what a finished brief looks like
├── LICENSE
└── README.md
```

## License

[GPL-3.0](LICENSE). Free to use, share and change. If you share a changed version, keep it under the same license.
