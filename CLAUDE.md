# CLAUDE.md

This repo is the source of the `croatian-web-copywriting` skill
(`skills/croatian-web-copywriting/`). Projects that use it (e.g. kontekst.hr) load it
read-only from the plugin, so every rule change is made here.

## Turning a copy correction into a rule

When the user corrects Croatian copy you wrote, in this repo or in a project that uses
the skill, the correction is a signal the skill is missing something. Don't just store
the fixed sentence. Store the pattern behind it, so the next draft avoids the whole
class of mistake.

Only language, tone, register and formatting corrections count. Factual or content
changes (a price, a service name, a date) are not rules.

1. **Fix the copy first.** Apply the correction, then look for the same pattern
   elsewhere on the page or in the diff and fix that too.

2. **Name the pattern.** Ask what the corrected line was doing wrong in general terms:
   which English habit it copied, which tone it slipped into, which convention it
   broke. One sentence, e.g. "negation-led claims calque 'We don't just X, we Y'".
   If you can't state it more broadly than the one sentence, it's a one-off preference:
   fix it and don't write a rule.

3. **Check the skill before adding.** Search `SKILL.md` and `references/` for a rule
   that already covers it.
   - Covered → the rule was too weak or too narrow. Sharpen the wording or add an
     example; don't add a duplicate.
   - Conflicts with an existing rule → ask the user which one wins.
   - New → write a new rule.

4. **Write the rule, not just the example.** Every rule has:
   - a bold one-line imperative (`**Drop the hedging modal.**`),
   - one or two sentences on *why* it sounds wrong in Croatian,
   - the user's own correction as the first ❌/✅ pair,
   - **at least two more ❌/✅ pairs you make up**, from a different domain than
     the original (not the same client) and, where it applies, a different copy type
     (headline vs. button vs. microcopy vs. meta),
   - the exceptions, if any (when the "wrong" form is actually right).

   The invented pairs are what make it generalize: they show the pattern, not the
   sentence. Keep them short and realistic.

5. **Put it in the right place.**
   - Applies to all Croatian web copy → `SKILL.md`, in the matching Workflow step (or a
     new step if it's a distinct idea), plus a line in **Copy review checklist**.
   - Applies to one copy type → the matching `references/*.md` file.
   - Only about one brand's voice (not Croatian in general) → that project's
     `AGENTS.md`/`CLAUDE.md`, not this skill.

6. **Add a regression check.** Add an assertion to the most relevant eval in
   `skills/croatian-web-copywriting/evals/evals.json`, or a new eval whose prompt
   would tempt the old mistake.

7. **Show before saving.** Show the user the rule and examples in a short block and
   save only after they say yes. A correction made once can be a matter of taste;
   the user decides whether it becomes a rule.

8. **Ship it.** Bump the patch version in all three manifests (`plugin.json`,
   `.claude-plugin/plugin.json`, `.cursor-plugin/plugin.json`), commit with a message
   like `Add rule: <pattern>`, and push. Projects pick it up from `main`. Remind the user
   that the synced skill on claude.ai has to be re-uploaded separately.
