---
name: croatian-web-copywriting
description: >-
  Writes and edits short-form website copy in natural, native-sounding Croatian —
  hero headlines, taglines, eyebrows, calls to action (pozivi na akciju), buttons,
  value propositions, and microcopy (form labels, placeholders, error and empty
  states, 404 pages, meta titles and descriptions, alt text). Use this WHENEVER you
  write, rewrite, translate, localize, or review any text that will appear on a
  Croatian-language website or app UI — even if the user never says "copywriting."
  Triggers include: "napiši hero / naslov / slogan", "smisli CTA / poziv na akciju",
  "tekst za naslovnu / landing / sekciju", "prevedi ovaj landing na hrvatski",
  "popravi ove gumbe", "kako da nazovem ovaj gumb", "treba mi tekst za formu / 404 /
  meta opis", or any request to make Croatian web copy sound less translated. Its
  whole job is copy that does NOT read as translated-from-English (no Title Case, no
  calqued slogans, one consistent Vi/ti register). For long-form blog posts or
  articles, use croatian-blog-writer instead.
---

# Croatian Web Copywriting

Short-form web copy is where Croatian sites most often fall apart — not on grammar,
but on *feel*. The text reads as if an English template were poured into Croatian:
Title-Cased headlines, calqued slogans ("Podignite svoje poslovanje na višu razinu"),
piled-up hype adjectives, and a register that slides between formal and informal on
the same page. A Croatian reader can't always name what's wrong, but they feel it —
the site sounds *prevedeno*, not *napisano*.

This skill is for writing copy that a Croatian reader experiences as written **by** a
competent Croatian professional, not localized into Croatian. It covers the small,
high-leverage text: hero headlines and leads, section eyebrows, CTAs and buttons,
value propositions, and microcopy (forms, errors, empty states, 404, meta tags). For
long-form articles and blog posts, use the `croatian-blog-writer` skill instead — it
owns the deep orthography/grammar guide; this skill assumes that baseline and focuses
on what is unique to *copy*.

## The one test that governs everything

Before shipping any line, ask:

> **Bi li ovo Hrvat stvarno rekao — ili to engleski govori s hrvatskim naglaskom?**
> (Would a Croatian person actually say this — or is it English speaking with a
> Croatian accent?)

Almost every rule below is a way of answering that question. The dominant failure
mode when writing Croatian web copy is **prevodilački hrvatski** (translationese):
sentences that exist only because an English original existed. The fix is always the
same — throw away the English sentence, keep the *idea*, and say the idea the way a
Croat would say it from scratch.

**Example — the whole skill in one rewrite:**

- Translationese: `Otključajte Svoj Puni Potencijal s Našim Rješenjima` ❌
  (Title Case · calque of "unlock your full potential" · empty "rješenja" ·
  pointless "svoj")
- Native: `Riješite to iz prve — bez lutanja i naknadnih troškova` ✅
  (sentence case · a real promise · concrete · sounds spoken)

## Workflow

Work in this order. Skipping step 1 is the most common mistake — register is a
decision, not a default, and everything downstream depends on it.

### 1. Lock the register before writing a word

Croatian forces a choice English doesn't: how you address the reader. Pick one for
the whole site and never drift. See `references/duh-hrvatskog.md` → "Oslovljavanje"
for the full decision guide. The short version:

| Register | When | CTA looks like | Feel |
|---|---|---|---|
| **Vi** (formal, plural) | Default for business, B2B, public sector, trades, anything selling trust | `Zatražite ponudu` | Professional, respectful |
| **ti** (informal, singular) | Youthful B2C, apps, startups, lifestyle brands | `Zatraži ponudu` | Friendly, peer-to-peer |
| **Impersonal** (no direct address) | When you want to dodge the choice or sound institutional | `Zatražite ponudu` / nominal phrasing | Neutral, safe |

**With Vi, capitalize every second-person form in direct address:** `Vi`, `Vam`, `Vas`,
`Vaš`, `Vaša`, `Vašu`, `Vašeg`… (`Pomažemo Vam`, `Vaša tvrtka`). Lowercase `vam/vas/vaš`
reads as careless in business copy. Also avoid stacking two pronouns in one clause —
name the object instead:
- ❌ `Pomažemo vam da vas kupci lakše pronađu` ✅ `Pomažemo Vam da kupci lakše pronađu Vašu tvrtku`

**Advise, don't lecture.** The company's voice is a consultant's, not a teacher's: prefer
`savjetujemo`, `predlažemo`, `pokazujemo` over `objašnjavamo`, which casts the reader as a
student.
- ❌ `U ovom tekstu objašnjavamo što utječe na vidljivost` ✅ `U ovom tekstu savjetujemo Vam na što se usredotočiti`

**Drop the hedging modal.** `mogu` + infinitive (`kako AI alati mogu razumjeti`) is a
calque of English "can/could" and weakens a plain statement. Use the direct verb.
- ❌ `provjeravamo kako AI alati mogu razumjeti Vašu ponudu` ✅ `provjeravamo kako AI alati razumiju Vašu ponudu`

**Translate the idea, not the consultant-speak.** "Highest-impact problem",
"identify blockers", "drive results" have no natural Croatian twin; a word-for-word
version (`problem koji ima najveći učinak`) and report verbs (`utvrdimo`) read like a report.
Say it the way you'd say it across the table.
- ❌ `Prvo utvrdimo što koči prodaju ili rad tima, a zatim riješimo problem koji ima najveći učinak.`
  ✅ `Prvo pronađemo što Vam usporava prodaju ili rad tima, a onda krenemo od onoga što pruža najveću vrijednost.`

The register dictates **every imperative on the site** (`Saznajte` vs `Saznaj`,
`Pošaljite` vs `Pošalji`). Mixing them is the #1 tell of unproofed copy — e.g. a site
that says `Zatražite ponudu` in the nav but `Pošalji upit` on the form button. Pick
one and sweep the whole site.

### 2. Find the real message before the clever one

For each block, answer in one plain Croatian sentence: *what does the reader get, and
why should they believe it?* Specifics beat adjectives — `200+ izgrađenih objekata`
earns more trust than `bogato iskustvo`. Lead with the reader's benefit, not the
company's self-description. Clarity outranks cleverness every time; a headline nobody
has to decode is already ahead.

### 3. Draft from the Croatian idea, not the English template

Write the line as if no English version existed. If you catch yourself translating a
known English pattern ("Get started", "Learn more", "Take it to the next level",
"We're committed to…"), stop — name the underlying intent and phrase it natively. The
catalogue of these patterns and their Croatian fixes is in
`references/duh-hrvatskog.md` → "Prevodilački hrvatski".

### 4. Apply the formatting non-negotiables

These are the mechanical tells that instantly mark copy as translated or unproofed.
They're cheap to get right and expensive to miss:

- **Sentence case for headlines**, never Title Case. `Gradimo pouzdano — od temelja do
  krova`, not `Gradimo Pouzdano — Od Temelja Do Krova`. Only the first word and proper
  nouns are capitalized. Title Case is the single loudest "translated from English"
  signal in Croatian.
- **Diacritics are mandatory** — č ć ž š đ. `Zatražite`, never `Zatrazite`. Stripped
  diacritics read as sloppy or spam, and they change meaning (`spas` ≠ `špas`).
- **CTAs are imperatives** in the chosen register: `Zatražite ponudu`, `Saznajte
  više`, `Pošaljite upit`, `Pogledajte projekte`. No `Klikni ovdje` ("click here").
- **Euro, not kuna** — Croatia is on the euro since 1 Jan 2023. `1.500 €` (symbol after
  the number, with a space). Kuna only ever appears in verbatim historical/legal facts.
- **Croatian number, date, currency, and quote formatting** — `10 000` or `10.000`
  (space or period thousands), `3,5 m` (decimal comma), `22. lipnja 2026.` (lowercase
  month in genitive), „ovako" (low-high quotes). Full rules in
  `references/duh-hrvatskog.md`.

### 5. Read it aloud, then cut

If you stumble reading a line, the reader will too. Cut hype adjectives
(`vrhunski`, `nevjerojatan`, `revolucionaran` rarely survive). Replace nominalizations
and bureaucratese with verbs: `vršimo uslugu prijevoza` → `prevozimo`; `realizacija
projekata` → `gradimo`. Shorter, more concrete, more spoken almost always wins.

Say each idea once. If you've already named the concrete mechanism, don't restate it as
a decorative echo — `svaki klijent ima svog stalnog referenta` already carries the
point; tacking on `bez prebacivanja od stola do stola` just repeats it. One concrete
statement beats a fact plus its synonym.

### 6. Say what you do, not what you don't

Negation-led copy (`Ne nudimo unaprijed zadano rješenje.`, `Ne krećemo od gotovog
paketa.`, `Ne isporučujemo samo stranicu`) is a calque of the English "We don't just X,
we Y" / "Not X, but Y" pattern. In Croatian it sounds defensive and translated, and it
makes the reader picture the thing you reject before the thing you offer. State the
positive action directly, and lead with the verb of what you actually do.

- ❌ `Ne nudimo unaprijed zadano rješenje. Najprije razumijemo problem, a zatim
  predlažemo što ima smisla napraviti.`
  ✅ `Prvo upoznamo Vaš posao i problem, a zatim predložimo rješenje po mjeri.`
- ❌ `Ne krećemo od gotovog paketa.` ✅ `Krećemo od Vašeg cilja.`
- ❌ `Ne koordinirate više dobavljača` ✅ `Jedan tim umjesto više dobavljača`
- ❌ `Ne nalazite svoje pitanje?` ✅ `Imate drugo pitanje?`
- ❌ `…, a ne samo jedan kanal.` ✅ `Gledamo sva tri mjesta zajedno.`

Two exceptions keep their negation: **honest caveats** that limit a promise
(`GEO ne jamči pojavljivanje u svakom AI odgovoru`), where accuracy beats positivity,
and **descriptions of the reader's problem** (`Kupac Vas ne pronađe`). The company's
own actions, offers and headings never open with `ne`.

### 7. Run the checklist

Before delivering, verify against the checklist at the bottom of this file.

## Reference files — read the one that matches the task

This SKILL.md is the hub; the depth lives in four references. Read the relevant one
*before* writing that element — don't reconstruct the rules from memory.

- **`references/duh-hrvatskog.md`** — *The spirit of Croatian.* The register decision
  (Vi/ti/impersonal) in full, the translationese catalogue (English patterns → native
  fixes), anglicisms and bureaucratese to avoid, tone (warmth without hype), and all
  formatting rules (sentence case, numbers, dates, euro, quotes, genitive-after-number
  agreement). **Read this for almost any task** — it's the soul of the skill.

- **`references/naslovi-i-pozivi.md`** — *Headlines & CTAs.* Read when writing or
  fixing hero headlines (H1/H2), eyebrows, leads, taglines, or any call to action /
  button. Formulas, patterns, a CTA verb bank, and many before/after examples drawn
  from real Croatian business copy.

- **`references/mikrokopija.md`** — *Microcopy & other elements.* Read when writing
  form labels/placeholders/buttons, validation and error messages, empty states, 404
  pages, success/confirmation messages, navigation labels, meta titles & descriptions,
  or image alt text. The small text that makes a site feel cared-for.

- **`references/jezicni-savjetnik.md`** — *Specific spelling/word-choice/punctuation
  rulings.* The "which form is correct" lookup — consult it whenever you hesitate over a
  specific word or mark: `sljedeći` vs `slijedeći`, `bit će` vs `biti će`, `zbog` vs
  `radi`, `od strane`, `s obzirom na to da`, `pogreška` vs `greška`, persiranje
  agreement (`Vi biste`, `Jeste li primili`), bullet-list punctuation, dates, slashes.
  Distilled from lektoriranje.org's Jezični savjetnik.

## Copy review checklist

Run every piece of copy through this before delivering:

- [ ] **Register is consistent** site-wide — every imperative is the same Vi *or* ti.
- [ ] **Vi forms capitalized** — `Vam`, `Vas`, `Vaš…` in direct address, never lowercase.
- [ ] **Nothing reads as translated** — no calqued slogan, no Title Case, no "Klikni ovdje".
- [ ] **Headlines are sentence case** and lead with the reader's benefit.
- [ ] **Diacritics intact** everywhere (č ć ž š đ).
- [ ] **CTAs are concrete imperatives** that say what happens next.
- [ ] **No negation-led claims** — say what you do, not what you don't (honest caveats
      and descriptions of the reader's problem excepted).
- [ ] **No empty hype** — claims are specific (numbers, names, facts) or cut.
- [ ] **Verbs over nominalizations** — no `vršenje`, `realizacija`, `u svrhu` filler.
- [ ] **Croatian formatting** — euro, decimal comma, lowercase-genitive dates, „quotes",
      correct case after numbers (`200 objekata`, `2 objekta`, `1 objekt`).
- [ ] **Read aloud cleanly** — you'd actually say it out loud.
- [ ] **Facts are real** — for an existing business, never invent stats, names, or claims;
      use only what the source provides.
