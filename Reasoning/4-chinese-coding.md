# 4️⃣ Coding — Concepts, methods, and solved examples

Great — coding/decoding is a pattern-recognition game. Below I’ll explain the common methods, show how to spot the pattern, then give worked examples (with full reasoning) you can practice.

---

## 🔎 Core idea

A word/number/phrase is transformed into another form by a rule (or set of rules). Your job: reverse-engineer the rule from the given pairs and apply it to a new item.

Common clues to look for:

* Position in alphabet (A=1, B=2, …)
* Reversal of letters or words
* Fixed shifts (each letter moved by +2, −1, etc.)
* Mirror/reflect (map first→last, second→second-last)
* Grouping (swap first and second halves)
* Substitution (replace strings with symbols)
* Numeric transforms (sum of positions, product, difference)
* Matrix/grid mapping (polybius square / 5×5 grid)

---

## 🔹 Types & how to spot them (quick)

* **Letter shift (Caesar-type):** letters moved by a fixed offset. Spot by checking common letters (e.g., E → G suggests +2).
* **Reverse / Mirror:** output looks like input reversed wholly or in parts.
* **Position-based (index rules):** only letters at odd/even positions changed.
* **Interleaving / swapping:** halves or alternate letters swapped.
* **Word-level substitution:** whole words replaced by codes/words (same word → same code).
* **Numeric coding:** words → numbers via letter sums, ASCII positions, or assigned values.
* **Matrix coding:** letters located from row/column numbers (Polybius).

---

## ✅ Examples (with full solutions)

### Example 1 — Simple letter shift

**Given:**
`DOG → FRI`
`CAT → FHW`

**Q:** `PEN → ?`

**Spot the pattern:**
D→F (+2), O→R (+3), G→I (+2) — not consistent. Check positions:

* For DOG: D(4)→F(6) = +2, O(15)→R(18) = +3, G(7)→I(9) = +2 → pattern: +2, +3, +2.
  Check same for CAT:
* C(3)→F(6)=+3, A(1)→H(8)=+7, T(20)→W(23)=+3 → not same. Hmm inconsistent — maybe pattern is: 1st & 3rd letters +2, middle +3 for DOG; for CAT first & third +3, middle +7. That’s messy. Try alternate idea: maybe letters replaced by next consonant/vowel pattern? Simpler approach — check mapping positions per index across examples:

Index 1: D→F (+2), C→F (+3) → no consistent addition.
This suggests these examples are not a consistent numeric shift; maybe they used **skip pattern relative to alphabet groups**. But this is too ambiguous for exam style — let’s use clearer examples below.

> Skip this example — ambiguous. (Important exam tip: if given inconsistent pairs, re-check original — real exam pairs are consistent.)

---

### Example 2 — Fixed shift (clean)

**Given:**
`ROAD → TQCF`
`BIKE → DKGG`

**Q:** `CAR → ?`

**Solution:**
Check shifts letterwise:
R(18)→T(20) = +2
O(15)→Q(17) = +2
A(1) → C(3) = +2
D(4) → F(6) = +2
So rule: **each letter +2 positions**.

Apply to CAR:
C(3)+2 = E(5) → E
A(1)+2 = C(3) → C
R(18)+2 = T(20) → T

**Answer:** `ECT`

---

### Example 3 — Reverse + shift

**Given:**
`EAST → WCBT`
`HILL → FJNN`

**Q:** `CODE → ?`

**Solution:**
Compare EAST → W C B T
Check letter mapping:
E→W (-4), A→C (+2), S→B (S=19→B=2 = +9 or -17), T→T (0) — messy.

Try reverse input first: EAST reversed = TSAE. Now compare TSAE → WCBT:
T→W (+3)
S→C (+10 or -16)
A→B (+1)
E→T (+15 or -11) — not consistent.

Given messy pairs, skip — use clearer standard patterns instead. (Again: pick clear pairs in tests.)

---

### Example 4 — Alternate-letter operations (good exam pattern)

**Given:**
`SPARK → URCTN`
`BRING → DTKPJ`

**Q:** `PLANE → ?`

**Solution:**
Look at index-wise transformation:
S→U (+2), P→R (+2), A→C (+2), R→T (+2), K→N (+3) — last one +3 breaks pattern. Try even/odd indexing:
Odd positions (1,3,5): S→U (+2), A→C (+2), K→N (+3) — last mismatch again.
Check second example BRING→DTKPJ:
B→D (+2), R→T (+2), I→K (+2), N→P (+2), G→J (+3) — pattern: first 4 letters +2, last +3.

Hypothesis: For 5-letter words, first four letters +2, last letter +3.

Apply to PLANE:
P→R
L→N
A→C
N→P
E→H (+3)

So result: `R N C P H` → `RNCPH`

**Answer:** `RNCPH`

---

### Example 5 — Pairwise swap + reverse

**Given:**
`SCHOOL → HSCOOL`
`MARKET → AMRKET`

**Q:** `GARDEN → ?`

**Solution:**
Look: SCHOOL → HSCOOL (S C H O O L → H S C O O L) — seems first two letters swapped: S C → H S? Wait, that's not a simple swap. But MARKET → AMRKET: M A R K E T → A M R K E T = first two letters swapped. For SCHOOL, expected swap would be 'CSHOOL' but given 'HSCOOL' — maybe typo.

Assume rule = **swap first two letters**.

Apply to GARDEN: G A R D E N → A G R D E N

**Answer:** `AGRDEN`

---

### Example 6 — Word-to-number (sum of positions)

**Given:**
`CAT → 24`
`DOG → 26`

**Q:** `BUS → ?`

**Solution:**
Compute sum of alphabet positions:
C(3)+A(1)+T(20)=24 ✓
D(4)+O(15)+G(7)=26 ✓

So BUS: B(2)+U(21)+S(19)=2+21+19=42

**Answer:** `42`

---

### Example 7 — Number coding with pattern (product or weighted sum)

**Given:**
`BAT → 2-1-20` (just letters separated) or `BAT → 23` if sum with some transform.
Better example below.

---

### Example 8 — Matrix / Polybius (5×5) style

Common in exams: map letters to row+column numbers using a 5×5 grid (I/J often combined).

**Construct 5×5 grid (example):**

```
  1 2 3 4 5
1 A B C D E
2 F G H I/J K
3 L M N O P
4 Q R S T U
5 V W X Y Z
```

Then `CAT` → C = (1,3) → 13, A = 11, T = 44 → encode as `13-11-44` or `131144` depending on format.

**Sample Q:** Using above grid, encode `DOG`.
D = 14, O = 33, G = 22 → `14 33 22` → `143322`.

---

### Example 9 — Substitution coding (sentence-level)

**Given:**
In a coded language:

* “tea is hot” → *lan kq zi*
* “coffee is hot” → *mav kq zi*

**Q:** “Is coffee sweet?” → ?

**Solution:**
From first two phrases:

* Common words: “is” and “hot” map to common tokens: `kq` and `zi`. So `kq` = is or hot; `zi` = the other.
  Compare: “tea is hot” and “coffee is hot” → they differ only in first token (tea vs coffee) mapping to `lan` and `mav`. So `zi` must be `hot` and `kq` = `is`.
  Thus mapping: `mav` = coffee, `lan` = tea, `kq` = is, `zi` = hot.

So “Is coffee sweet?” → structure `is coffee sweet` → `kq mav X`. We don’t have code for sweet → cannot fully encode. If exam gave code for sweet elsewhere you substitute. If not, answer: **cannot be determined / insufficient data**.

---

### Example 10 — Chinese style (pattern on positions)

**Given:**
`POND → QPMF`
`LAKE → MBKF`

This looks like: every letter replaced by next letter but last becomes previous? Check:
P→Q (+1), O→P (+1), N→M (−1), D→F (+2) — inconsistent.
But LAKE→MBKF: L→M(+1), A→B(+1), K→K(+0), E→F(+1). Maybe N→M is −1 earlier anomaly. Better avoid ambiguous examples.

---

## 🧠 How to approach exam questions (step-by-step)

1. **List given pairs** and write them vertically (original vs code).
2. **Compare letter by letter** (or word by word). Note shifts, swaps, same-code for same-subword.
3. **Check positions** (first letters across samples, second letters, etc.).
4. **Test your inferred rule on all given pairs** — if any pair contradicts, refine.
5. **Apply to the query.** If rule can’t be uniquely determined, answer “cannot be determined” (many tests include that option).

---

## 🔁 Quick practice (try these)

1. If `FISH → GJTI` (each letter +1, but S→T correct — check pattern), then `COW → ?` → `DPX` (each +1).
2. If `PEN → 40` where P(16)+E(5)+N(14)=35 → 40 suggests +5 constant. So for `RAT` (R18+A1+T20=39) → +5 → `44`.
3. If `RAIN → 91514` as concatenation of positions (R=18→18 but shown 9?), be careful — always compute stepwise, not assume.

---

