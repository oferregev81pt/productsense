# AI PM Hub — Claude plugins

Claude plugins for product managers, from The AI PM Hub.

## Plugins

- **[product-sense-interview](plugins/product-sense-interview)** — an interactive
  PM interview coach for product-sense / product-design questions, built
  strictly on the frameworks in *Cracking the PM Interview* (Gayle Laakmann
  McDowell & Jackie Bavaro). Coaches one step at a time and saves a structured
  write-up.
- **[pm-mock-interview](plugins/pm-mock-interview)** — runs a realistic,
  pressure-tested PM product-design mock interview: plays a tough but fair
  interviewer, then gives a rubric scorecard, a hire verdict, and one
  concrete drill to work on next.

## Install

### Claude Code

```
/plugin marketplace add oferregev81pt/productsense
/plugin install product-sense-interview@ai-pm-hub
/plugin install pm-mock-interview@ai-pm-hub
```

Or, without the marketplace, copy the skill folder you want directly into
your personal skills directory:

```bash
cp -r plugins/product-sense-interview/skills/product-sense-interview ~/.claude/skills/
cp -r plugins/pm-mock-interview/skills/pm-mock-interview ~/.claude/skills/
```

(Use `.claude/skills/` inside a specific project instead of `~/.claude/skills/`
to scope it to that project.)

### Cursor (and other Agent-Skills-compatible tools)

```
npx skills add oferregev81pt/productsense
```

Or copy the rule file(s) you want into your project's rules directory:

```bash
mkdir -p .cursor/rules
cp cursor/product-sense-interview.mdc .cursor/rules/
cp cursor/pm-mock-interview.mdc .cursor/rules/
```

The `product-sense-interview` rule references the worked examples at
`plugins/product-sense-interview/skills/product-sense-interview/references/book-examples.md`
— copy that file alongside it (or adjust the relative path) if you move it
elsewhere.

## Usage

### product-sense-interview

Give it a product question to practice:

> **You:** Help me practice — design an alarm clock for blind users.
>
> **Agent:** That's a "Design a product" question. I'll walk you through:
> clarifying questions → structure → users/customers → use cases → how
> today's products fall short → improvements → wrap-up. First — what
> clarifying questions would you ask the interviewer?

Answer each step as it comes; the coach reacts before moving on. When you're
done, you'll have a saved `product-sense-<question-slug>.md` write-up with
your full structured answer, coaching notes, and a model answer for
comparison.

#### The three frameworks

| Type | Steps |
|------|-------|
| **Design a product** | clarify → structure → users/customers → use cases → current-product weak spots → improvements → wrap up |
| **Improve a product** | goal & user → problems → solve → implement → validate |
| **Favorite product** | problems it solves → what makes it neat → vs. alternatives → how you'd improve it |

### pm-mock-interview

Tell it which product you want to be asked about:

> **You:** Run a mock interview on improving Spotify.
>
> **Agent:** [plays interviewer, delivers a slightly ambiguous prompt, then
> stays in character through clarify → users → use cases → solutions →
> prioritize → metrics, with one pushback along the way]

At the end you get a rubric scorecard (1-4 per area with evidence), an
overall hiring verdict, and the single most important thing to drill next.
It also supports a single-section drill, and design/favorite-product or
other question-type variants — just ask.

## Credits & license

`product-sense-interview` frameworks adapted from *Cracking the PM Interview*
by Gayle Laakmann McDowell and Jackie Bavaro. MIT license.
