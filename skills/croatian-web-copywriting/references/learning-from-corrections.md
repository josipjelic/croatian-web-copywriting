# Learning from corrections

When the user corrects Croatian copy you wrote, the skill was missing something.
Don't just remember the fixed sentence. Find the pattern behind it and store it as a
rule with fresh examples, so the next draft avoids the whole class of mistake, in this
project and in the next one.

This applies to **language, tone, register and formatting** corrections only. Factual
or content changes (a price, a service name, a date, a claim the client doesn't make)
are not rules.

## 1. Fix the copy first

Apply the correction. Then look for the same pattern elsewhere on the page, in the
diff or in the rest of the site's copy, and fix it there too. Mention what else you
changed.

## 2. Name the pattern

Say in one sentence what the corrected line was doing wrong *in general*: which
English habit it copied, which tone it slipped into, which convention it broke.

- `Ne nudimo gotova rješenja.` → `Krećemo od Vašeg cilja.` →
  "negation-led claims calque 'We don't just X, we Y'"
- `Pomažemo vam` → `Pomažemo Vam` → "Vi forms are capitalized in direct address"

If you can't state it any more broadly than the one sentence, it's a one-off
preference: apply it, say so, and don't write a rule.

## 3. Check what's already there

Search `SKILL.md`, the `references/` files and the project's own copy rules (see
step 6) for a rule that already covers it.

- **Already covered** → the rule was too weak or too narrow. Sharpen the wording or
  add an example instead of writing a duplicate.
- **Conflicts with an existing rule** → ask the user which one wins.
- **New** → write a new rule.

## 4. Write the rule, not just the example

Every rule has:

- a bold one-line imperative (`**Drop the hedging modal.**`),
- one or two sentences on *why* it sounds wrong to a Croatian reader,
- the user's own correction as the first ❌/✅ pair,
- **at least two more ❌/✅ pairs you invent**, from a different industry than the
  project and, where the rule allows it, a different kind of copy (headline, button,
  form microcopy, meta description),
- the exceptions, if any (when the "wrong" form is actually right).

The invented pairs make it generalize: they show the pattern, not the sentence. Keep
them short, realistic and in the same register as the rule requires.

Template:

```markdown
**<Imperative in one line.>** <Why it sounds translated or off in Croatian.>
- ❌ `<user's original>` ✅ `<user's correction>`
- ❌ `<invented, other industry>` ✅ `<fix>`
- ❌ `<invented, other copy type>` ✅ `<fix>`

Exception: <when the pattern is fine>.
```

## 5. Ask before saving

Show the rule in the template above and ask one short question: save it, and where
(step 6 proposes the default). A single correction can be a matter of taste; the user
decides whether it becomes a rule. If the user has said to save without asking, skip
the question and just report what you saved.

## 6. Save it where it will be found next time

Pick the first option that works:

**a) The skill's source repo** (`josipjelic/croatian-web-copywriting`), when the rule
is about Croatian web copy in general and you can push to that repo (it's cloned in
the session, or you can attach it with push access).

- General rule → `SKILL.md`, in the matching Workflow step (or a new step if it's a
  distinct idea), plus one line in **Copy review checklist**.
- Rule for one kind of copy → the matching `references/*.md` file.
- Add an assertion to the most relevant eval in `evals/evals.json`, or a new eval whose
  prompt would tempt the old mistake.
- Bump the patch version in all three manifests (`plugin.json`,
  `.claude-plugin/plugin.json`, `.cursor-plugin/plugin.json`), commit as
  `Add rule: <pattern>` and push to `main`, which every project installs from.
- Tell the user that the copy of the skill uploaded to claude.ai, if they use one,
  has to be re-uploaded separately.

**b) The current project**, when the rule is only about this brand's voice, or when
you can't push to the skill repo. Add it under a `## Croatian copy rules` heading in
the project's `CLAUDE.md` (or `AGENTS.md` if that's where the project keeps agent
instructions; create the heading if it's missing), and commit it with the rest of the
change. Tell the user it applies to this project only, and offer the rule as an issue
or PR for the skill repo if it's general.

**c) No file access** (a plain chat): give the user the rule block to paste into the
skill or their project instructions, and say clearly that it hasn't been saved.

## Using saved project rules

Before writing copy in a project, read its `## Croatian copy rules` section if there
is one. Those rules apply on top of this skill and win where they conflict.
