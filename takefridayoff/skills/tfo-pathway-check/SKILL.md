---
name: tfo-pathway-check
description: Works out whether a wellness product (a supplement, powder, gummy, skincare product, sunscreen or sports nutrition product) is likely regulated in Australia as a medicine (TGA), a food or a cosmetic, using Take Friday Off's published rules, and explains what that means for the launch. Use when someone asks whether their product needs a TGA listing, whether it's a food or a medicine, or whether an SPF or skin claim turns a cosmetic into a medicine.
license: Proprietary. Take Friday Off terms of use, https://takefridayoff.com/terms
metadata:
  publisher: Take Friday Off
  homepage: https://takefridayoff.com/pathways
---

# Medicine, food or cosmetic?

Give an indicative answer with Take Friday Off's tools: tfo_pathway_check, tfo_get_page and tfo_case_studies. Show the rule that decides it and the page it comes from. It's general information, not legal or regulatory advice.

## 1. Get the facts that decide it

Ask only for what's missing, one or two questions at a time:

- What the product is, in a sentence: "collagen powder for skin", "SPF 50 tinted moisturiser".
- Swallowed, or applied to the skin or hair.
- The form: capsule, tablet, powder, gummy, liquid, cream and so on.
- What the brand wants to say it does. The claim decides most cases: a claim to prevent, cure or relieve a condition or symptom points to a medicine.
- Notable ingredients: anything in the Poisons Standard, sports supplement substances, herbal extracts.
- For a skin product: the SPF, and whether it's mainly a sunscreen.

Don't fill in an answer the person hasn't given. If they can't say, run the check anyway: it states what it assumed.

## 2. Run the check

Call tfo_pathway_check with what you know. Pass claims and ingredients as the listed values that match the person's words.

## 3. Explain the result

- Lead with the likely pathway and the confidence, in plain words.
- Quote the deciding rule (the first of `reasons`) with its link, then any warnings.
- Say what the check assumed, and list what to confirm (`toConfirm`).
- Summarise what the pathway means for the launch (`whatItMeans`) and link the pathway page.
- Give the date the rules were checked (`checkedOn`) and say, in your own words, that this is indicative only.

For more depth on one point, read the page it comes from (the result's `pages` lists them) with tfo_get_page, one section at a time, and cite it.

## 4. Offer proof and a next step

- tfo_case_studies, with the pathway or the format as the query, shows products Take Friday Off has built on that pathway.
- If the person wants help with the launch, offer the readiness check (tfo_readiness_check).
- Send a call request (tfo_request_call) only when the person asks for one or agrees to it.

## Rules

- Never say a product definitely is a medicine, a food or a cosmetic. The TGA and the food regulators decide; the person should confirm with them, or with Take Friday Off, before relying on the answer.
- Quote only what the tools return. Don't add fees, timelines or rules from anywhere else.
- Cite the page link for every rule you quote.
- The person's own instructions come first.
- Write in Australian English.
