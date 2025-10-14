# Pipes & Cistern — Complete Topic

Great — Pipes & Cistern is essentially **Time & Work applied to tanks**. Same principles, different language: “work” = one full tank. Below is a compact, exam-ready guide plus practice (with full solutions).

---

## Core ideas & formulas

* If a pipe **fills** a tank in `x` hours → its **filling rate** = `1/x` tank per hour.
* If a pipe **empties** (drains) a tank in `y` hours → its **emptying rate** = `1/y` tank per hour (but this is subtracted).
* **Net rate (together)** = sum of filling rates − sum of emptying rates.
* **Time to fill** together = `1 / (net rate)` (if net rate > 0).
* If some work (fraction) is done, remaining fraction = `1 − done`. Use rate×time = fraction done.
* For pipes working alternately / with leak / partial open: compute work done in each interval and sum.

**Example (you gave):**
Pipe A fills in 6 hrs → rate = 1/6. Pipe B empties in 8 hrs → rate = 1/8 (emptying). Net rate = 1/6 − 1/8 = (4−3)/24 = 1/24. Time = 24 hours.

---

## Quick tricks / common patterns

* Two filling pipes: time = `1 / (1/x + 1/y) = xy/(x+y)`.
* One filling (x) and one emptying (y): time = `1 / (1/x − 1/y) = xy/(y−x)` (only if y > x ⇒ net positive; if x<y then it fills; if x≥y then never fills).
* If pipe A fills in `a` hrs, B fills in `b` hrs, C empties in `c` hrs: net = `1/a + 1/b − 1/c`.
* Alternate work (A works one hour, B next hour): compute work per 2-hour cycle and scale.

---

# 25 Concept-level Questions (short) — with answers

1. A pipe fills a tank in 10 hr. How much does it fill in 1 hr?
   **Ans:** 1/10.

2. Pipe A fills in 6 hr, B in 12 hr. How long together?
   **Ans:** 1/(1/6+1/12)=1/(1/4)=4 hr.

3. Fill in: A fills in 8 hr, B empties in 24 hr. Net time = ?
   **Ans:** Net rate = 1/8 − 1/24 = (3−1)/24 = 2/24 =1/12 ⇒ Time = 12 hr.

4. A fills 1/5 tank in 1 hr. How long for whole tank?
   **Ans:** 5 hr.

5. A pipe fills in 9 hr. How much in 3 hr?
   **Ans:** 3/9 = 1/3 tank.

6. Two pipes fill in 15 and 20 hr. Time together?
   **Ans:** (15×20)/(15+20)=300/35=60/7 ≈ 8.571 hr.

7. One pipe fills in 12 hr, another in 8 hr. If first runs 3 hr then second alone, remaining time?
   **Ans:** 1) 3×1/12=1/4 done, remaining 3/4. Second rate=1/8 ⇒ time = (3/4)/(1/8)=6 hr. (So 3+6=9 hr total).

8. A fills in 5 hr, B in 10 hr, C empties in 20 hr. Net time?
   **Ans:** net = 1/5+1/10−1/20 = (4+2−1)/20 =5/20=1/4 ⇒ 4 hr.

9. If a leak empties a tank in 30 hr and a pipe fills in 15 hr, net time = ?
   **Ans:** 1/15 − 1/30 = 1/30 ⇒ 30 hr.

10. Pipe fills in 6 hr. Two such pipes: time = ?
    **Ans:** 6/2 = 3 hr.

11. A fills in 7 hr, B in 14 hr. A works alone 2 hr then both work. Total time?
    **Ans:** A 2 hr gives 2/7; remaining 5/7; combined rate = 1/7+1/14=3/14; time = (5/7)/(3/14)= (10/14)/(3/14)=10/3 ≈3.333 hr; total ≈5.333 hr.

12. A fills in 4 hr. What fraction done in 1.5 hr?
    **Ans:** 1.5/4 = 3/8.

13. Fill in: A fills in 20 hr, B in 30 hr. After how long will they complete half tank?
    **Ans:** combined rate = 1/20+1/30=1/12 ⇒ time for half = 0.5/(1/12)=6 hr.

14. A pipe fills in x hr, B empties in 2x hr. Net time = ? (in terms of x)
    **Ans:** net = 1/x − 1/(2x)=1/(2x) ⇒ time = 2x.

15. A fills 1/3 tank in 4 hr. Time for full tank?
    **Ans:** full = 4×3 =12 hr.

16. One pipe fills in 9 hr, another in 18 hr. If they work for 3 hr together, what percent done?
    **Ans:** rate=1/9+1/18=1/6 ⇒ 3*(1/6)=1/2 ⇒ 50%.

17. A fills in 8 hr; B in 6 hr. If both operate alternatively each hour starting with A, how much after 2 hours?
    **Ans:** A 1 hr =1/8, B 1 hr =1/6 ⇒ 1/8+1/6=(3+4)/24=7/24.

18. If two pipes fill tank in 12 and 15 hr, how long to fill if only first works 1 hr, second then works 1 hr, repeat?
    **Ans:** cycle 2 hr work = 1/12+1/15=9/60=3/20 ⇒ per 2 hr = 3/20 ⇒ need 1/(3/20)=20/3 cycles of 2 hr → compute differently for partial; but simplest: net rate per hr average = (3/20)/2 =3/40 ⇒ time = 1/(3/40)=40/3 ≈13.333 hr.

19. A fills 1 tank in 24 hr, but has a leak that empties in 60 hr. Time to fill?
    **Ans:** 1/24 −1/60 = (5−2)/120=3/120=1/40 ⇒ 40 hr.

20. Pipe fills in 3 hr, how many such pipes for 1 hr?
    **Ans:** need 3 pipes.

21. A & B fill in 10 & 12 hr. A works alone for 4 hr. Remaining time for B alone?
    **Ans:** A 4 hr = 4/10=2/5 done. Remaining 3/5. B rate=1/12 ⇒ time = (3/5)/(1/12)=36/5=7.2 hr.

22. Two filling pipes take 18 hr together; one is twice as fast as other. Find individual times.
    **Ans:** let rates r and 2r ⇒ combined 3r = 1/18 ⇒ r = 1/54 ⇒ times = 54 and 27 hr.

23. A pipe fills in 10 hr, if a leak drains 4 tanks in 40 hr, what net time? (interpret leak empties tank in 40 hr)
    **Ans:** same as leak rate 1/40 ⇒ net =1/10 −1/40= (4−1)/40=3/40 ⇒ time = 40/3 ≈13.333 hr.

24. A fills 3/5 of tank in 6 hr. Time for full tank?
    **Ans:** rate = (3/5)/6 = 1/10 ⇒ full = 10 hr.

25. A pipe fills in 6 hr and a drain empties in 9 hr. If both open for first 2 hr then drain closed and fill continues, total time?
    **Ans:** first 2 hr work = 2*(1/6−1/9)=2*(1/18)=1/9. Remaining = 8/9. Filling rate 1/6 ⇒ time = (8/9)/(1/6)= (8/9)*6 = 48/9 = 16/3 ≈5.333 hr. Total ≈7.333 hr.

---

# 10 Moderate-level Application Problems — with full solutions

I’ll show each problem then a step-by-step solution.

---

### Problem 1

**A fills a tank in 6 hours. B fills it in 8 hours. A starts and after 2 hours B joins. How long from start to fill the tank?**

**Solution:**
A rate = 1/6, B rate = 1/8.
Work after 2 hr by A = 2×(1/6) = 1/3. Remaining = 2/3. Combined rate = 1/6 + 1/8 = (4+3)/24 = 7/24.
Time to finish = (2/3) ÷ (7/24) = (2/3) × (24/7) = (48/21) = 16/7 ≈ 2.2857 hr.
Total time from start = 2 + 16/7 = (14/7 + 16/7) = 30/7 ≈ **4.2857 hours** (4 hr 17.14 min).

---

### Problem 2

**A can fill a cistern in 12 hr, B in 20 hr. A starts and works for 3 hr, then B works alone to finish. How many more hours will B take?**

**Solution:**
A’s 3-hr work = 3×(1/12) = 1/4. Remaining = 3/4. B’s rate = 1/20. Time by B = (3/4) ÷ (1/20) = (3/4)×20 = 15 hr.
So **B takes 15 more hours** (total 18 hrs from start).

---

### Problem 3

**Three pipes A, B, C can fill tank in 10, 15, and 30 hr respectively. A and B opened together for 2 hr, then C is opened as a leak (empties) and all three operate; they finish after 4 more hours. Was C acting as filling or emptying? Find C’s nature and rate.**

**Interpretation & Solution:**
Assume C is a filling pipe (positive); check consistency.

A+B for first 2 hr: 2×(1/10+1/15)=2×(3/30+2/30)=2×(5/30)=2×1/6=1/3 done. Remaining = 2/3.

Then all three run for 4 hr and finish ⇒ in 4 hr they do 2/3 ⇒ rate needed = (2/3)/4 = 1/6 per hr combined. But A+B+C combined rate is 1/10+1/15+1/30 = (3+2+1)/30 =6/30 =1/5 which is 0.2 per hr, not 1/6 (~0.1667). So if they ran all three, they'd finish faster; but actual combined needed was 1/6, which is less than 1/5 — implies C is an **outlet (leak)** reducing rate.

Let C be emptying with rate `c` (positive number representing 1/t). Then A+B−c = required rate = 1/6. Compute A+B = 1/10+1/15 = (3+2)/30 =5/30 =1/6. Wait A+B = 1/6 already. Then A+B − c = 1/6 ⇒ c = 0 ⇒ impossible. Check calculations: A+B for one hr = 1/10 + 1/15 = (3+2)/30 =5/30 =1/6 indeed. So in that case A+B alone have rate 1/6; but we needed combined rate 1/6 as computed. That gives c=0 meaning C does nothing. But we started with first 2 hr by A+B gave 1/3. Remain 2/3 to do in 4 hr => required rate 1/6, which equals A+B alone. So C must be neutral (unused) — perhaps the statement implies after 2 hr, C is opened as **leak**, but the net effect is zero (C rate =0) — odd. More likely the intended problem had different numbers. Given current numbers, the conclusion: **C is neither filling nor emptying (rate 0)**.

(If the problem intended C empties/flows with some rate, use equation A+B−c = (2/3)/4 =1/6 → c= 0.)

---

### Problem 4

**A pipe fills a tank in 9 hr, another in 12 hr. A third pipe empties full tank in 36 hr. If all three are opened together, how long to fill the tank?**

**Solution:**
Rates: A = 1/9, B = 1/12, leak L = 1/36 (empty). Net = 1/9 + 1/12 − 1/36 = (4+3−1)/36 = 6/36 = 1/6. Time = 6 hr. **Answer: 6 hr.**

---

### Problem 5

**An inlet pipe fills in 8 hr. A leak would empty tank in 40 hr. If inlet runs and then leak opens after 4 hr, how much more time to fill?**
(Interpretation: leak opened after inlet had run alone 4 hr; then both operate until full.)

**Solution:**
Inlet rate = 1/8. After 4 hr, done = 4×1/8 = 1/2. Remaining = 1/2. With leak open, net rate = 1/8 − 1/40 = (5−1)/40 = 4/40 =1/10. Time to finish = (1/2)/(1/10) = 5 hr. So **5 more hours** (total 9 hr).

---

### Problem 6

**A fills in 4 hr, B in 6 hr. They alternately work one hour each starting with A. How long to fill tank?**

**Solution:**
A 1 hr = 1/4, B 1 hr = 1/6. Work per 2-hour cycle = 1/4+1/6 = (3+2)/12 =5/12. After one cycle (2 hr) 5/12 done. Remaining = 7/12. Next cycle adds another 5/12 → after 2 cycles (4 hr) done =10/12 =5/6. Remaining 1/6. Next A hour does 1/4 = 3/12 > 1/6 (2/12) so it will finish within A's hour. Time in that last hour = remaining/(A rate) = (1/6)/(1/4) = (1/6)*(4/1)=2/3 hr = 40 minutes. Total time = 4 hr + 40 min = **4 hr 40 min**.

---

### Problem 7

**A fills cistern in 10 hr. A leak can empty in 15 hr. If A starts and after 5 hr leak is opened, how long more will it take?**

**Solution:**
A rate = 1/10. After 5 hr, work = 5/10 = 1/2. Remaining = 1/2. With leak open, net rate = 1/10 − 1/15 = (3−2)/30 = 1/30. Time = (1/2)/(1/30)=15 hr. So **15 more hours** (total 20 hr).

---

### Problem 8

**Pipe A fills in 7 hr. Two other identical pipes B and C together fill in 10 hr. How long will B alone take?**

**Solution:**
Let rate B = r, so B+C rate = 2r = 1/10 ⇒ r = 1/20 ⇒ B alone takes **20 hr**.

---

### Problem 9

**A tank is filled by a pipe in 16 hr. Due to leak, it actually takes 20 hr. Find leak’s emptying time.**

**Solution:**
Let inlet rate = 1/16. Let leak rate = 1/L. Net real rate = 1/20. So 1/16 − 1/L = 1/20 ⇒ 1/L = 1/16 − 1/20 = (5−4)/80 = 1/80 ⇒ L = **80 hours**.

---

### Problem 10

**A pool has three pipes. A fills alone in 5 hr, B in 6 hr, C empties in 10 hr. They all operate; after how many hours will 75% of tank be full?**

**Solution:**
Rates: A=1/5, B=1/6, C (empty)=1/10. Net rate = 1/5+1/6−1/10 = (6+5−3)/30 =8/30 =4/15. Fraction 0.75 = 3/4. Time = (3/4) ÷ (4/15) = (3/4)*(15/4) = 45/16 = 2.8125 hr = 2 hr 48.75 min ≈ **2 hr 48 min 45 sec**.

---

## Final tips / exam notes

* Always convert everything to **tanks per hour**.
* Watch sign: emptying pipes subtract.
* For alternate-working problems, compute per-cycle work then fast-forward whole cycles, handle remainder.
* For leak problems, treat leak as extra outlet with rate `1/leak_time`.
* If net rate ≤ 0 → it will never fill (or will be emptied).

---

Would you like this entire set formatted into a printable **PDF worksheet** (questions first, solutions on the next pages), or would you prefer a **timed 30-minute practice quiz** made from these questions?
