# Mikrokopija i ostali elementi — microcopy & other text

The small text that makes a site feel cared-for: forms, errors, empty states, 404s,
confirmations, navigation, meta tags, alt text. Microcopy is where register
consistency and anti-translationese matter *most*, because these strings are the ones
most often left in default English or machine-translated. All examples assume the
**Vi** register (switch to `ti` per `duh-hrvatskog.md` if the site is informal).

**Contents**
1. [Obrasci — form labels, placeholders, buttons](#1-obrasci)
2. [Poruke o pogreškama — validation & errors](#2-poruke-o-greskama)
3. [Potvrde — success & confirmation](#3-potvrde)
4. [Prazna stanja i 404](#4-prazna-stanja-i-404)
5. [Navigacija](#5-navigacija)
6. [Meta naslovi i opisi (SEO)](#6-meta)
7. [Alt tekst i pristupačnost](#7-alt-tekst)
8. [Kolačići i pristanak](#8-kolacici)

---

## 1. Obrasci

Keep labels short and in the noun form; keep buttons as register-consistent
imperatives.

**Labels** — concise, capitalized first word only:
- `Ime i prezime` · `E-mail adresa` · `Broj telefona` · `Poruka` · `Tema upita`

**Placeholders** — show the *format*, don't repeat the label. Never put the label only
in the placeholder (it vanishes on focus and hurts accessibility).
- Label `E-mail adresa`, placeholder `ime@tvrtka.hr`
- Label `Broj telefona`, placeholder `091 234 5678`

**Buttons** — name the outcome, in register:
- ✅ `Pošaljite upit` · `Zatražite ponudu` · `Pošaljite poruku`
- ❌ `Pošalji` (bare/informal if the site is Vi) · `Submit` · `Potvrdi` (vague)

**Optional/required & helper text** — small, plain:
- `Nije obavezno` (optional) · `Obavezno polje` (required)
- Helper: `Odgovaramo radnim danom u roku od 24 sata.`

**Privacy reassurance** under a form lifts trust:
- `Vaše podatke koristimo isključivo za odgovor na upit.`

---

## 2. Poruke o greškama

The golden rule of error microcopy: **say what happened and how to fix it — never
blame the user, never make them feel stupid.** Croatian error copy especially must
avoid the cold administrative tone (`Greška: nevažeći unos`).

| Situation | Cold/translated ❌ | Human Croatian ✅ |
|---|---|---|
| Empty required field | `Polje je obavezno!` | `Upišite svoje ime` / `Unesite e-mail adresu` |
| Bad email | `Nevažeći e-mail` | `Provjerite e-mail adresu — čini se da nešto nedostaje` |
| Bad phone | `Greška u formatu` | `Upišite broj u formatu 091 234 5678` |
| Message too short | `Poruka prekratka` | `Napišite nam malo više — barem nekoliko riječi` |
| Server/submit failure | `Error 500` | `Nešto je pošlo po zlu. Pokušajte ponovno za koji trenutak.` |
| Network | `Network error` | `Nema veze s internetom. Provjerite vezu i pokušajte ponovno.` |

Notes:
- Prefer the imperative fix (`Unesite…`, `Provjerite…`) over the noun verdict
  (`obavezno polje`). It tells the reader what *to do*.
- Keep the register: Vi → `Provjerite`; ti → `Provjeri`.
- One exclamation mark max per page. Croatian copy with `!` everywhere reads as
  shouting or translated marketing.
- A direct imperative usually beats an embedded question (`provjerite je li točno
  upisana`) — shorter, and it sidesteps question-forming pitfalls. When you *do* ask a
  question, never open with `da li`; front the verb + `li`: `Trebate li…?`, `Je li…?`
  (see `duh-hrvatskog.md` → „Upitne rečenice: glagol naprijed").

---

## 3. Potvrde

Confirmations should close the loop warmly and set the next expectation.

- Form sent: `Hvala! Vaš upit je zaprimljen — javljamo se u najkraćem roku.`
- Quote requested: `Zahtjev za ponudu je poslan. Odgovaramo radnim danom u roku od 24 sata.`
- Newsletter: `Prijava je uspješna. Dobrodošli!`
- Avoid the bare `Uspjeh.` / `Poslano.` — it's correct but cold; add the human beat and
  the next step.

---

## 4. Prazna stanja i 404

**Empty states** explain why it's empty and what to do — they're an opportunity, not a
dead end:
- Search no results: `Nema rezultata za „<pojam>". Pokušajte s drugim pojmom.`
- Empty list/portfolio filter: `Za ovaj filter još nemamo projekata. Pogledajte sve
  realizacije.`

**404 pages** — admit it plainly, keep the tone, offer a way back. Don't be cute at
the reader's expense:
- Heading: `Stranica nije pronađena`
- Body: `Tražena stranica ne postoji ili je premještena.`
- CTA: `Vratite se na naslovnu` · `Pogledajte usluge`

**500/maintenance:**
- `Trenutačno radimo na stranici. Vratite se uskoro.`

---

## 5. Navigacija

Nav labels are nouns, short, sentence case, consistent with the site's vocabulary:
- `Naslovna` · `O nama` · `Usluge` · `Projekti` · `Kontakt`
- `Home` → `Naslovna` or `Početna`, never `Dom`.
- Keep them parallel: all nouns (`Usluge`, `Projekti`) — don't mix in a verb phrase.

Footer/utility links: `Uvjeti korištenja` · `Politika privatnosti` · `Pravila o
kolačićima` · `Sva prava pridržana`.

---

## 6. Meta

Meta titles and descriptions are copy too — written for a Croatian reader scanning
search results, not stuffed with keywords.

**Title** (~50–60 chars): primary thing + place/brand, separated by `—` or `|`.
- `L Projekt — Graditeljstvo i proizvodnja betona | Pleternica`
- `Betonara — proizvodnja i dostava betona | Pleternica`

**Description** (~150–160 chars): a real sentence that earns the click — what you offer
+ a concrete differentiator. Natural Croatian, no keyword salad.
- `Vlastita betonara u Pleternici — standardni, armirani, pumpani i specijalni beton.
  Miješalice 5–11 m³, pumpe 21 i 36 m. Brzo, kvalitetno i povoljno.`

Same rules as the rest of the site: sentence-style, diacritics, euro, no Title Case,
chosen register.

---

## 7. Alt tekst

Image alt text describes the image for screen readers and search — a plain Croatian
description, not a keyword dump and not "slika ...".
- ✅ `Betonska miješalica L Projekta na gradilištu u Požegi`
- ❌ `slika1`, `beton beton dostava betona Pleternica jeftino`
- Decorative images get empty alt (`alt=""`), not a description.

---

## 8. Kolačići

Croatian sites need a GDPR cookie notice; keep it plain and honest, not a wall of
legalese.
- Banner: `Koristimo kolačiće kako bi stranica radila ispravno i kako bismo
  poboljšali vaše iskustvo.`
- Buttons: `Prihvati sve` · `Odbij` · `Postavke` (these are conventionally `ti`/neutral
  imperatives on most Croatian sites — keep them consistent with each other even if the
  body copy is Vi).
- Link: `Saznajte više u Pravilima o kolačićima.`
