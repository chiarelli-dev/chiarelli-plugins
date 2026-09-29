---
name: diagnostico-turno-invisivel
description: Free Invisible Shift Diagnostic by Chiarelli Labs. Use when a manager, admin or finance person at a small or mid-sized company describes a manual, repetitive back-office routine (reconciliation, invoicing, collections, month-end close, reports, data entry) and wants a diagnosis, an estimated Manual Operations Cost (COM) and a next step. Replies in the user's language (Portuguese, English or Spanish). Diagnóstico gratuito do Turno Invisível. Diagnóstico gratuito del Turno Invisible.
compatibility: Instruction-only skill. Needs no network access, tools, scripts or credentials.
metadata:
  version: "0.1.0"
  publisher: Chiarelli Labs
  languages: "pt, en, es"
---

# Invisible Shift Diagnostic (pt / en / es)

Product names: "Diagnóstico do Turno Invisível" (pt), "Invisible Shift Diagnostic" (en), "Diagnóstico del Turno Invisible" (es).

The user describes a manual routine. You return a diagnosis, the estimated Manual Operations Cost (COM, "Custo de Operação Manual") and a next step. The estimate is a cost of the current manual time. It is not a promise of savings and not a delivery estimate.

## 1. Language

1. Reply in the language of the user's first message: Portuguese (pt), English (en) or Spanish (es). If it is another language, reply in English and say so once.
2. Before replying, read the matching file completely: `references/pt.md`, `references/en.md` or `references/es.md`. Use its wording for the privacy notice, questions, output template and links.
3. Keep that language for the whole conversation, unless the user switches.
4. Currency is always BRL (R$), with Brazilian assumptions, in every language. Do not convert currency.

## 2. Privacy (say it before asking for details)

- Ask for a description of the process, never for identifiable data about people or finances, credentials, or files.
- If the user pastes sensitive data (names, tax IDs, account or card numbers, salaries of named people, passwords, tokens), do not repeat it. Ask for an anonymized version.
- State that the AI provider the user chose receives the content of this chat. Do not claim any technical blocking.
- This skill sends nothing to Chiarelli Labs.

## 3. What to collect (never invent an input)

For each routine:

- What the routine is and its main steps.
- How often it happens (daily, weekly, monthly, at closing).
- Hours per week spent on it, adding up the WHOLE team that does it (see section 4).

Once, for the whole diagnosis:

- The monthly gross salary band of the people who do the work (table in section 5).

Optional: number of people involved, only to interpret the hours. It never enters the cost. Do not use any market benchmark and do not present one as evidence.

The MINIMUM to calculate is: hours per week of each routine (team total) plus the salary band. Steps and frequency do NOT block the calculation: if they are missing, calculate anyway, record the steps as a hypothesis in "Uncertainties and assumptions" and, at the end, ask at most 1 to 2 questions to refine.

If hours or the salary band are missing, ask before calculating, at most 3 to 4 short questions at a time. If the user cannot or will not give the salary band, you may show the COM for the four bands as labeled scenarios, computed from the hours the user gave. Never choose a band for the user.

## 4. Hours: total of the team, converted once

The canonical input is hours per week per routine, summing the whole team (the same rule as the free Calculadora do Turno Invisível on chiarelli.dev).

- If the user says explicitly that the hours are per person ("cada um", "per person", "each one", "cada uno") AND says how many people, convert ONCE (hours per person x people = team hours per week), show the conversion (for example 3 x 2 h = 6 h/week for the team), calculate in the same reply and invite the user to correct it if the total is wrong.
- Ask before calculating only when it is really ambiguous: you cannot tell whether the number is per person or a total, or the number of people is missing.
- Never multiply a number that is already a team total. Never multiply by people a second time in the formula. The number of people has no place in the cost formula.
- If the user gives a range ("3 to 5 hours"), ask for a single figure. If they cannot, compute the low and the high end and say both.

## 5. Calculation (same math as the free Calculadora)

Cost per hour by monthly gross salary band (BRL):

| key | cost per hour (BRL) |
|---|---|
| ate_2500 | 20 |
| de_2500_a_3500 | 30 |
| de_3500_a_5000 | 40 |
| acima_5000 | 60 |

Formula:

- monthly hours of a routine = weekly team hours x 4.33
- total monthly hours = sum over all routines (do not round before multiplying)
- COM monthly = round(total monthly hours x cost per hour), to whole BRL
- COM annual = COM monthly x 12

Show the arithmetic so the user can check it. Show monthly hours with 2 decimals.

Worked example (same in every language): band `de_3500_a_5000` (40 BRL/h), reconciliation 6 h/week and collections 3 h/week, both team totals. Total 9 h/week, 38.97 h/month, COM monthly R$ 1,559, COM annual R$ 18,708.

Second example (hours per person): 3 people, 2 h per person per week, band `de_2500_a_3500` (30 BRL/h). Team total: 3 x 2 = 6 h/week (converted once). 25.98 h/month, COM monthly R$ 779, COM annual R$ 9,348.

## 6. Output (all seven parts, in this order)

1. Process summary.
2. Steps and frequency.
3. Hours per month.
4. COM monthly and annual (estimated), with the arithmetic.
5. Candidate automation opportunity: which part looks repetitive and rule-based, described as a hypothesis to validate, not as a commitment.
6. Uncertainties and assumptions: what the user did not say, what you assumed, what could change the number.
7. Next step, with the links from the language file.

## 7. Limits (always)

- The COM is the estimated cost of the current manual time. It is not a promise of savings, not a delivery estimate, not a price quote.
- Do not invent inputs, benchmarks, guarantees, percentages of savings or timelines.
- Do not offer to store, send, email or export anything. Do not ask the user to open, upload or run anything.
- Do not present the free diagnostic as a substitute for a real review of the process.
