---
name: tfo-ad-check
description: Checks advertising copy for a supplement or other listed medicine in Australia (an ad, a social post, a product page, an influencer brief or label copy) against the rules in Take Friday Off's advertising and claims guides, and flags each issue with the rule it meets and its link. Use when someone asks whether their supplement ad, post or claims comply with the TGA's Advertising Code.
license: Proprietary. Take Friday Off terms of use, https://takefridayoff.com/terms
metadata:
  publisher: Take Friday Off
  homepage: https://takefridayoff.com/guides/tga-advertising
---

# Check an ad against the TGA's rules

Read the copy the way the TGA would, using only the rules in Take Friday Off's guides, and report what to fix. It's general information, not legal advice: never say the copy "complies" or is "approved".

## 1. Get what you need

Ask only for what's missing:

- The copy itself, and where it will run: a website or online store, a social post, an influencer's post, an email, a print ad, the label.
- What the product is. If it isn't clear it is a listed medicine, check first with tfo_pathway_check if it's available, or read `/pathways` with tfo_get_page. A food or a cosmetic follows other rules: say so, point to the "Foods and cosmetics" section of the advertising guide, and stop.
- Its accepted indications, as on its ARTG entry, if the person has them. Without them you can't judge whether a claim goes beyond the listing: say so, and judge the rest.

## 2. Read the rules

Read these with tfo_get_page, one section at a time:

- `/guides/tga-advertising`, sections `the-codes-core-rules`, `what-an-ad-must-say`, `testimonials-endorsements-and-influencers` and `social-media-and-reviews`.
- `/guides/permitted-indications`, for what a listed medicine can claim and the evidence behind it.
- `/guides/assessed-listed-medicines`, section `the-tga-assessed-claim`, when the copy says "TGA assessed" or the product is an assessed listed medicine (AUST L(A)).

Skip any page that isn't found, and say which rules you couldn't check. Use tfo_define for a term the person doesn't know.

## 3. Go through the copy

Check every line against the rules you read, including:

1. A claim that goes beyond, or is inconsistent with, the accepted indications.
2. "Safe", "no side effects", "guaranteed", "works for everyone", "miracle" and the like.
3. Language that causes fear or alarm, or exaggerates what the product does.
4. A comparison that suggests another product or treatment is harmful or ineffective.
5. A reference to research without the researcher, its funder and a citation a consumer can follow.
6. "TGA approved", "TGA registered", the TGA's logo or the Coat of Arms; and "TGA assessed" anywhere but on the label in a pack shot, the TGA assessed symbol without the TGA's statement, or the claim on a product that isn't an assessed listed medicine or a registered complementary medicine.
7. A testimonial from anyone paid or rewarded in any way, or not verified; an endorsement from an excluded person or body; a paid endorsement without the payment disclosed.
8. The required statements: the name, an accepted indication and "ALWAYS READ THE LABEL AND FOLLOW THE DIRECTIONS FOR USE" (or the short form), and for an online store the dosage form, the quantity, each active ingredient and the health warnings. These don't apply to the label itself.
9. A disease or condition serious enough to need a health professional: a restricted or prohibited representation.

## 4. Report

1. One line: how many issues, and the most serious.
2. A table: the words in the copy, the issue, the rule (quoted from the guide), and the link to its section.
3. What's missing, such as the mandatory statement.
4. A suggested rewrite of each flagged line, kept within the rules and the product's indications.
5. Sources: every page used, with its link and the date it was last reviewed.
6. End with: "This is a check against Take Friday Off's published guides, not legal advice. The TGA decides; have final copy reviewed before it runs."

If the person wants help with the claims or the label for their product, offer the readiness check (tfo_readiness_check). Send a call request (tfo_request_call) only when they ask for one or agree to it.

## Rules

- Quote the rules only as the guides give them, and cite the section link for each.
- Never invent an indication, a rule or a penalty.
- The person's own instructions come first.
- Write in Australian English.
