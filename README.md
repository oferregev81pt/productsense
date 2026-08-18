# product-sense-interview

An interactive PM interview coach for product-sense / product-design
questions, built strictly on the frameworks in *Cracking the PM Interview*
(Gayle Laakmann McDowell & Jackie Bavaro).

It detects which of the book's three question types you're facing —
**Design a product**, **Improve a product**, or **Favorite product** — states
the framework it will run, then coaches you through it one step at a time:
you answer, it gives short targeted feedback, then moves you to the next
step. No lecture, no full model answer dumped up front — the value is in your
reps. At the end it saves a structured write-up of the session.

Stays strict to the book's toolkit: Customer/Users First (CUF), users →
use cases → solutions, and the three step-by-step frameworks below. It won't
substitute in outside frameworks like RICE or CIRCLES.

## Install

### Claude Code

```
/plugin marketplace add oferregev81pt/product-sense-interview
/plugin install product-sense-interview@product-sense-interview
```

Or, without the marketplace, copy the skill folder directly into your
personal skills directory:

```bash
cp -r skills/product-sense-interview ~/.claude/skills/
```

(Use `.claude/skills/` inside a specific project instead of `~/.claude/skills/`
to scope it to that project.)

### Cursor (and other Agent-Skills-compatible tools)

```
npx skills add oferregev81pt/product-sense-interview
```

Or copy the rule file into your project's rules directory:

```bash
mkdir -p .cursor/rules
cp cursor/product-sense-interview.mdc .cursor/rules/
```

The rule references the worked examples at
`skills/product-sense-interview/references/book-examples.md` — copy that file
alongside it (or adjust the relative path) if you move it elsewhere.

## Usage

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

## The three frameworks

| Type | Steps |
|------|-------|
| **Design a product** | clarify → structure → users/customers → use cases → current-product weak spots → improvements → wrap up |
| **Improve a product** | goal & user → problems → solve → implement → validate |
| **Favorite product** | problems it solves → what makes it neat → vs. alternatives → how you'd improve it |

## Credits & license

Frameworks adapted from *Cracking the PM Interview* by Gayle Laakmann
McDowell and Jackie Bavaro. MIT license.
