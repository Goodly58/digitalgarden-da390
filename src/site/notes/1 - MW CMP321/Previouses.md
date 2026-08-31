---
{"dg-publish":true,"permalink":"/1-mw-cmp-321/previouses/"}
---

### 📋 Past-Exam Index (which is which)

| #       | Type         | Label                                            |
| ------- | ------------ | ------------------------------------------------ |
| **E1**  | 🏁 **FINAL** | Final Exam (A)                                   |
| E2      | 📝 Midterm 1 | Midterm 1 (A)                                    |
| E3      | 📝 Midterm 2 | Midterm 2 (A)                                    |
| E4      | 📝 Midterm 1 | Midterm 1 (B)                                    |
| **E5**  | 🏁 **FINAL** | Final Exam (B) — 11 Pages                        |
| E6      | 📝 Midterm 2 | Midterm 2 (B)                                    |
| E7      | 📝 Midterm 2 | Midterm 2 (C)                                    |
| E8      | 📝 Midterm 1 | Midterm 1 — Spring 2020 (Online)                 |
| E9      | 📝 Midterm 1 | Midterm 1 — Spring 2021 (Online)                 |
| E10     | 📝 Midterm 1 | Midterm 1 — Fall 2021                            |
| E11     | 📝 Midterm 1 | Midterm 1 — Spring 2022                          |
| **E12** | 🏁 **FINAL** | Final A — May 2020                               |
| **E13** | 🏁 **FINAL** | Final B — Unknown Semester (Grammar-Heavy)       |
| **E14** | 🏁 **FINAL** | Final C — Unknown Semester (BNF & Attr Grammars) |
| E15     | 📎 Appendix  | Reconstructed Questions from Student Answers     |
| E16     | 📝 Midterm 1 | Midterm 1 — Spring 2019                          |
| **E17** | 🏁 **FINAL** | Final Exam — Spring 2021                         |

> 🏁 **Finals (6 papers):** E1, E5, E12, E13, E14, E17 — these are the highest-priority references for the upcoming Final on Mon May 11.
> 📝 **Midterms:** the remaining (M1: E2, E4, E8, E9, E10, E11, E16 · M2: E3, E6, E7) are still useful for topic coverage since the Final is comprehensive.

---

## 🎯 Final Exam — Study Plan & NEW Content (Days F1–F4)

> [!danger] 🗓 Exam: **Monday, 11 May 2026 · 11 AM (Section 01)** · *(Section 02: Sat 9 May, 11 AM)*
> Confirmed via iLearn course `_95399_1` (Programming Languages S26 Section 01) — confirmed by Dr. Pasquier on **May 3, 2026** ("Course evaluation + Final exam + Office hours") and **May 6, 2026** ("Final exam scope").
> - **Comprehensive** — covers all topics from beginning to end (M1 + M2 + new content)
> - **120 minutes for 100 marks** · 1-mark-per-minute pacing rule
> - Same format as midterms — essay (2-6 marks, 3-7 min), design ("formulate"), derivation ("apply") · **No MCQs anymore**
> - Today is **Thu May 7** · exam is **4 days away** ⏰

### Scope — only what's NEW since M2 (per Pasquier's "Final exam scope" email — May 6, 2026)

> [!success] ✅ NEW for Final (not covered in M1 or M2 plans)
> Per Pasquier's actual scope email — the **strikethrough formatting** in the original email indicates exclusions. Only the un-struck items below are in scope.
> - **Topic 6 — OOP basics** — Python classes, attributes, methods only (the *parts discussed in class*). **NO inheritance, NO abstract classes, NO `super()`, NO `@abstractmethod`** — Pasquier explicitly crossed those out.
> - **Topic 8a — Generators** — generator functions (`yield`), generator expressions `(expr for x in iter)`, lazy data types · NOT iterators (crossed out)
> - **Comprehensions** — list `[…]`, set `{…}`, dict `{k:v …}`, generator `(…)` · was excluded from M2 per Thani's note, NOW in scope
> - **Additional HOFs** — `accumulate`, `takewhile`, `dropwhile`, `chain` from `itertools` (mentioned in Week 15 agenda)
> - **Efficient Python idioms** (per Pasquier's "Efficient Python, examples/tests" email Apr 29, 2026):
>     - `Counter` from collections — letter frequency one-liner
>     - `Counter(list1) == Counter(list2)` — same elements check (hashable, faster)
>     - `sorted(list1) == sorted(list2)` — same elements (orderable)
>     - `dict3 = {**dict1, **dict2}` — merge dicts via kwargs unpacking
>     - `list(set(alist))` — dedupe in O(N)
>     - tuple > list when no mutation; parallel assignment for swap

> [!failure] ❌ Confirmed OUT of scope (per Pasquier's strikethrough scope email + Week 15 agenda + CLO recap)
> - **Inheritance** — crossed out in Topic 6 of scope email
> - **Abstract classes** (and `@abstractmethod`, `abc.ABC`) — crossed out in Topic 6
> - **Iterators** — crossed out in Topic 8 (custom iterator classes via `__iter__`/`__next__`). Note: `next()`/`iter()`/StopIteration as built-in functions used IN given code are still ok per E6 Q3a precedent
> - **Regular expressions** — Topic 9 entirely crossed out · Week 15 email confirmed "we won't have time"
> - **Declarative Programming / Prolog / CLP / Chapter 16** — Topic 10 entirely crossed out · CLO recap: "out of scope this semester"
> - **Annotated types** — Week 15 agenda: "we've skipped many sections already e.g., annotated types and decorators"
> - **Decorators** — Week 15 agenda (same email)
>
> Rule: *"whatever we studied in class is included, unless specified otherwise, and whatever material we skipped is out of scope"* (Pasquier, May 6).


---

## 🎯 Midterm 2 — Study Plan & Filtered TOC

> [!danger] 🗓 Exam: **Saturday, 2 May 2026 · 2:30–3:30 PM (online)**
> Confirmed by Dr. Pasquier on **Apr 19, 2026** ("Confirmed (Re: Midterm #2 exam date/time)").
> - **Online** (both sections), Respondus Monitor required
> - **Reduced number of questions** (instead of 15 min extra time) — pace yourself
> - Today is **Sun Apr 26**, exam is **6 days away** ⏰

### Scope (per Pasquier's email — 5 tutorials)

> [!success] ✅ In scope — five tutorials
> 1. **Fundamentals of Python** (Pasquier 01 / [[1 - MW CMP321/W7 C1\|W7 C1]]) — interpreter, dynamic typing, variables, slicing, raw strings, complex numbers, `id()`, `is` vs `==`, parallel assignment, imports
> 2. **[[1 - MW CMP321/W12 C2\|C2 — Sequences & Collections]]** (Pasquier 02) — lists, tuples, dicts, sets, named tuples, hashing, mutability
> 3. **[[1 - MW CMP321/W13 C3\|C3 — Flow Control & Repetition]]** (Pasquier 03) — if/while/for, `range`, `enumerate`, `zip`, walrus, loop-`else`
> 4. **[[1 - MW CMP321/W13 C4\|C4 — Functions & Lambda]]** (Pasquier 04) — multiple returns, default/keyword args, `*args`/`**kwargs`, scoping (LEGB), closures, decorators, no-overloading, type annotations
> 5. **[[1 - MW CMP321/W14 C7\|C5 — Higher-Order Functions]]** (Pasquier 07) — `map`/`filter`/`reduce`, `accumulate`, `starmap`, `@cache`/`@lru_cache`, `partial` (NOTE: comprehensions out of scope per Thani's note)
>
> Rule: *"anything discussed in detail in class is examinable (and conversely)"*. Re-watch class recordings if unsure.

> [!failure] ❌ Out of scope
> - **Tutorial 5** (Classes & Inheritance) — not formally covered → no OOP, no `__init__`, no inheritance, no diamond problem, no abstract classes
> - **Tutorial 6** (Exceptions & I/O) — not formally covered
> - **Tutorial 8** (Iterators & Generators beyond what `map`/`filter`/`reduce` already produce) — Pasquier explicitly said "the next Tutorial #8 is also out of scope, even if we start before the midterm"
> - **Comprehensions** (list/dict/set/generator) — *per Thani's note*. Past papers often say "use HOFs but NOT comprehensions" anyway, so focus on `map`/`filter`/`reduce` to express the same patterns.
> - **Regular expressions** — not yet taught
>
> Pasquier's email mentioned "we discussed Python classes, methods, and attributes in many places" — but per Thani's reading of class content, this is **not** examinable. Skip every OOP question in the past papers.

### 📅 Where you should be today

| Date                | Day       | Phase                                                  | Notes                                           |
| ------------------- | --------- | ------------------------------------------------------ | ----------------------------------------------- |
| Sun Apr 26          | Day 1     | C1 Fundamentals warm-up + C2 — Sequences & Collections |                                                 |
| Mon Apr 27          | Day 2     | C3 — Flow Control & Repetition                         |                                                 |
| **Tue Apr 28**      | **Day 3** | **C4 — Functions, Lambda, Closures, Scoping**          | **← you are here**                              |
| Wed Apr 29          | Day 4     | C7 — Higher-Order Functions (no comprehensions)        |                                                 |
| Thu Apr 30          | Day 5     |                                                        | ← Active study done by EOD (3 days before exam) |
| Fri May 1           | —         | Review review                                          |                                                 |
| **Sat May 2**       | **EXAM**  | 🎯 **2:30–3:30 PM online** — Respondus Monitor         | Parser project work                             |
| Sun May 3–Tue May 5 | post-exam | Parser project (due Tue May 5, 11:11 PM)               |                                                 |

### 📚 Day-by-Day Plan

#### Day 1 — Tue Apr 28 · C1 Fundamentals warm-up + C2 Sequences & Collections

##### Morning — C1 Fundamentals warm-up (~30–45 min)

- [ ] Skim [[1 - MW CMP321/W7 C1\|W7 C1 lecture notes]] — focus on what's NEW vs what's already drilled in M1: dynamic typing semantics, parallel assignment / unpacking, `id()`, `is` vs `==`, complex numbers, raw strings, slicing edge cases, `import` aliases, `exec`/`eval`
- [x] Core practice — pick whichever you feel weakest on:
    - [x] [[#Exam 1: Question 4 — Python Strings & Slicing|E1 Q4]] — raw strings, complex `j+2j`, slicing
    - [x] [[#Exam 5: Question 2 — Raw Strings, Assignment & Slicing|E5 Q2]] — raw strings, `x='y'` Python vs C++, slicing
    - [x] [[#Exam 8: Question 2 — Dynamic Typing, Type Inference & Python Expressions|E8 Q2]] — dynamic typing, `auto x=1` vs `x=1`, slicing
    - [x] [[#Exam 11: Question 2 — lsub Function, auto vs x=1 & pprint|E11 Q2]] (b) — `auto` vs `x=1` type inference
- [x] Additional reps from M1 prep — slicing / dynamic typing / unique-expressions duplicates (knock these out fast):
    - [x] [[#Exam 2: Question 5 — Python Expressions & Slicing|E2 Q5]] — `x,y=[1,2j]` unpacking, complex, dynamic typing, slicing
    - [x] [[#Exam 5: Question 5 — Python Expressions & Slicing|E5 Q5]] — duplicate of E2 Q5
    - [x] [[#Exam 9: Question 1 — Slicing, Reasons for Studying PLs, Case Sensitivity, Orthogonality & Compilation|E9 Q1]] — only the slicing sub-part
    - [x] [[#Exam 9: Question 2 — Dynamic Typing, Python Expressions, Slicing & Format|E9 Q2]] — dynamic typing, slicing, `.format()` with `divmod`
    - [x] [[#Exam 10: Question 2 — String Slicing & Dictionary Comprehension|E10 Q2]] — only (a) string slicing (skip (b) dict comprehension ❌)
    - [x] [[#Exam 16: Question 2 — Dynamic Typing, Unique Expressions, Slicing & Format|E16 Q2]] — duplicate of E8 Q2 / E9 Q2
    - [x] [[#Exam 16: Question 6 — Multiple Choice (Abstraction, Features, Type Check, MI)|E16 Q6]] — only **MCQ #3** (`type(s) is not str`); skip #1 (abstraction = M1), #2 (mixed M1), #4 (MI = OOP)
- [x] Self-check: what does `j+2j` evaluate to · why `n1 is n2` may be `True` for small ints/strings (caching/interning) · what makes a string "raw"

##### Main — C2 Sequences & Collections

- [ ] Re-read [[1 - MW CMP321/W12 C2\|W12 C2 lecture notes]] (lists, tuples, dicts, sets, hashing, mutability)
- [x] Practice — past exam questions:
    - [x] [[#Exam 1: Question 5 — Python Data Structures|E1 Q5]] — swap/unpack, dicts, sets
    - [x] [[#Exam 4: Question 1 — Python Expressions & Function Calls|E4 Q1]] — mixed: `len(str(x).split('.')[-1])` (C4) · `1+7j` (C1) · `'say "hi"!'` (C1) · `[1]*10` repetition (C2) · `range(20,4,-4)` lazy (C3)
    - [x] [[#Exam 4: Question 2 — Python Strings, Tuples & Dictionaries|E4 Q2]] — palindrome, duplicates, dict grouping
    - [x] [[#Exam 7: Question 1 — Python Expressions & Uniqueness|E7 Q1]] — uniqueness via `len(t)!=len(set(t))` 
    - [x] [[#Exam 7: Question 2 — Python Expressions & Dictionary Grouping|E7 Q2]] — dict grouping pattern
    - [x] [[#Exam 8: Question 3 — List Replacement, Built-in Shadowing, Closures & Lambdas|E8 Q3]] (a) — list slicing replacement
    - [x] [[#Exam 11: Question 2 — lsub Function, auto vs x=1 & pprint|E11 Q2]] (a) — `lsub` list slicing replacement (≈ E8 Q3(a))
- [x] Self-check: `l[1] = [...]` vs `l[1:2] = [...]` · `==` vs `is` · why lists can't be dict keys · what `__hash__`/`__eq__` are for

> [!success]- Self Check Solution
> (1)
> 
> l[1] = [...] is indexing it will make the element a sublist with whatever is inside as the elements
> 
> l[1:2] = [...] will perform slicing and will replace l's elements with whatever is inside the RHS list. It will extend if the size of the RHS is greater than the size of LHS (>1 element).
> 
> (2) == returns true when two elements are equal each other in value (even if types differ: 1 == 1.0 returns true), otherwise false. is returns true when LHS has same memory location as RHS, in other words have the same reference to an object in memory ([1,2,3] is [1,2,3] returns false, \== would've returned true), otherwise false.
> 
> 3) Dict keys must be hashable. Lists are mutable: if you mutate a list after using it as a key, its hash would change, breaking the hash-table invariant.
> 
> 4) __hash__(self) returns an integer hash of the object, used by sets/dicts to bucket it and __eq__(self,other) is equivalent to the \== operator, checks self\==other

#### Day 2 — Tue Apr 28 · Flow Control & Repetition (C3)

- [ ] Re-read [[1 - MW CMP321/W13 C3\|W13 C3 lecture notes]] (if/while/for, range, zip, walrus, loop-`else` — skip the comprehensions section)
- [x] Practice — past exam questions:
    - [x] [[#Exam 3: Question 1 — Python Expressions & Scripting|E3 Q1]] — mixed C2/C3 expressions, scripting
    - [x] [[#Exam 3: Question 2 — Boolean Expressions & Zip|E3 Q2]] — `zip` + boolean expressions
    - [x] [[#Exam 7: Question 3 — Comparisons (== vs is) & Pythonic Code|E7 Q3]] — `==` vs `is`, Pythonic style
- [x] Pythonic-pattern drill: chained comparisons, ternary, short-circuit eval, `enumerate` vs `range(len(...))`

1. **Chained comparisons** — what does `1 < x < 10` do, and why is that not allowed in C++/Java?
2. **Ternary** — write a one-line expression that returns `'even'` if `n % 2 == 0` else `'odd'`.
3. **Short-circuit eval** — what does `0 or 5` return? What does `5 or 0` return? Why?
4. **`enumerate` vs `range(len(...))`** — which is more Pythonic for iterating with an index, and why?



> [!success]- Solution
> (1) 1<x<10 checks if x is between 1-10 (both exclusive)
> (2) return 'even' if n%2\==0 else 'odd'
> (3) 
> a or b: if a is truthy, return a; else return b.    <span class="neon-highlight">OR WANTS FIRST GOOD VALUE</span>
> a and b: if a is falsy, return a; else return b. <span class="neon-highlight">STOP AT FIRST FALSY VALUE</span>
> **0 or 5: 5** <-- returns 5
> **5 or 0: 5** <-- returns 5
> 
> if it was 
> 0 and 5: 0
> 5 and 0: 0
> 
> (4) enumerate(...) is more pythonic because range(len(...)) is verbose and less readable and mimics c++ style rather than python.


#### Day 3 — Wed Apr 29 · Functions, Lambda, Closures, Scoping (C4 — full)

- [ ] Re-read [[1 - MW CMP321/W13 C4\|W13 C4 lecture notes]] **end-to-end** (it's all in scope)
- [x] Practice — functions/lambda/multi-return:
    - [x] [[#Exam 1: Question 6 — Python Functions & Recursion|E1 Q6]] — recursive minmax, docstrings
    - [x] [[#Exam 3: Question 3 — Functions: Multiple Returns, Overloading & `len`|E3 Q3]] — no-overloading, `len`
    - [x] [[#Exam 5: Question 3 — Recursive minmax & Fibonacci via reduce|E5 Q3]] (a) — recursive `minmax` (similar to E1 Q6, fresh rep)
    - [x] [[#Exam 10: Question 3 — Multiple Returns, Dictionary Dispatch & Closures|E10 Q3]] — dict dispatch
    - [x] [[#Exam 11: Question 2 — lsub Function, auto vs x=1 & pprint|E11 Q2]] (c) — `pprint` with f-strings
    - [x] [[#Exam 11: Question 3 — Multiple Returns, **call**, Sorting & Closures|E11 Q3]] — `__call__`, sorting
- [ ] Practice — closures/scoping/shadowing (the most-asked M2 topic):
    - [x] [[#Exam 6: Question 2 — Functional Programming, Closures & Expressions|E6 Q2]] — closures, lambdas
    - [x] [[#Exam 7: Question 4 — Function Parameters, F-Strings & Closures|E7 Q4]] — params, f-strings, closures
    - [x] [[#Exam 8: Question 3 — List Replacement, Built-in Shadowing, Closures & Lambdas|E8 Q3]] (b) — built-in name shadowing (`list = 1` breaks `list()`)
    - [x] [[#Exam 8: Question 3 — List Replacement, Built-in Shadowing, Closures & Lambdas|E8 Q3]] (c–d) — closures, lambdas
    - [x] [[#Exam 9: Question 3 — mix() Function, Closures, Lambdas & Sorting|E9 Q3]] — `mix()`, closures, sorting
    - [x] [[#Exam 16: Question 3 — lsub Function & Square Class|E16 Q3]] (a) — `lsub` function
- [x] Practice — recursion + map-based patterns (C4/C5 bridge):
    - [x] [[#Exam 16: Question 5 — Tail-Recursive lzip, map-based zip & Efficiency|E16 Q5]] — tail recursion, map-based `zip`, iterator efficiency
- [x] Self-check: 3 conditions for a closure · `nonlocal` vs `global` · LEGB rule · mutable-default trap

1. **Three conditions for a closure** (state them).
2. **`nonlocal` vs `global`** — what does each do, and when do you use them?
3. **LEGB rule** — what does it stand for, and what's the order of name resolution?
4. **Mutable-default-argument trap** — what's the bug, and how do you fix it?


> [!success]- Solution
> (1)
> 
> 1. nested function
> 2. inner function references outer function variable
> 3. outer function returns inner function
> 
> (2)
> Without these keywords:
> 
> Reading from outer/global scope: works fine (LEGB resolves it).
> Writing to a variable inside a function: creates a NEW local variable (shadows outer scope).
> With these keywords:
> 
> nonlocal x — tells Python "the x I'm assigning to refers to the nearest enclosing function's scope (E), not a new local."
> global x — tells Python "the x I'm assigning to refers to the module-level / global scope (G)."
> 
> ```
> x = 1   # global
> 
> def outer():
>     x = 2   # local to outer
>     
>     def inner_no_keyword():
>         x = 3   # creates NEW local in inner; outer's x stays 2
>     
>     def inner_nonlocal():
>         nonlocal x   # refers to outer's x
>         x = 3        # modifies outer's x → 3
>     
>     def inner_global():
>         global x   # refers to module-level x
>         x = 99     # modifies global x → 99
> ```
> 
> 
> (3)
> Order is L->E->G->B
> L -> local
> E ->  enclosing 
> G -> global
> B -> built-in (last thing that is checked)
> 
> (4)
> ```
> def add_item(item, items=[]):
>     items.append(item)
>     return items
> 
> print(add_item("a"))   # ['a']
> print(add_item("b"))   # ['a', 'b']  ← bug! Same list reused
> 
> ##FIX:
> def add_item(item, items=None):
>     if items is None:
>         items = []          # fresh list each call when no items provided
>     items.append(item)
>     return items
> ```




#### Day 4 — Wed Apr 29 · Higher-Order Functions (C7, no comprehensions) ← active study done by EOD

- [ ] Re-read [[1 - MW CMP321/W14 C7\|W14 C5 lecture notes]] — focus on HOFs (`map`/`filter`/`reduce`), decorators, `itertools`. **Skip the Comprehensions section.**
- [x] Practice — `map`/`filter`/`reduce`:
    - [x] [[#Exam 1: Question 8 — Functional Programming (map/filter/reduce)|E1 Q8]]
    - [x] [[#Exam 3: Question 5 — Functional Programming & Higher-Order Functions|E3 Q5]]
    - [x] [[#Exam 6: Question 3 — Higher-Order Functions: reduce & map|E6 Q3]]
    - [x] [[#Exam 7: Question 5 — Higher-Order Patterns & Expressions|E7 Q5]]
- [x] Practice — advanced HOFs (skip any comprehension sub-parts; do HOF rewrites only):
    - [x] [[#Exam 5: Question 3 — Recursive minmax & Fibonacci via reduce|E5 Q3]] (b) — Fibonacci via `reduce`
    - [x] [[#Exam 8: Question 5 — Expressions, Comprehensions & Higher-Order Concepts|E8 Q5]] — **skip (b) "use a comprehension"** sub-parts; do (a) and (c) HOF parts only
    - [x] [[#Exam 10: Question 5 — Higher-Order Expressions & Patterns|E10 Q5]]
    - [x] [[#Exam 11: Question 5 — Higher-Order Patterns, Expressions & reduce|E11 Q5]]
    - [x] [[#Exam 17: Question 2 — Templates, range() & Memoized Fibonacci|E17 Q2]] (b) `range()` · (c) memoised Fibonacci
    - [x] [[#Exam 17: Question 3 — Comprehension/HOF Rewrite & Fibonacci via reduce|E17 Q3]] — **only the (ii) "classic HOFs" rewrite**, skip the (i) comprehension rewrite
- [ ] Re-do [[1 - MW CMP321/HW4\|HW4]] questions A & B (already submitted, just re-derive)

#### Day 5 — Thu Apr 30 · Mock Exam + Formula Sheet + Weak-Topic Clean-Up

- [ ] **Mock exam (timed, ~1 hour)** — open **Midterm2-Xpaper.pdf** from iLearn → *Course Documents → Sample Exam Papers*. No notes. Mark yourself afterwards. **Skip any OOP / class / inheritance / exception questions** — they're out of scope.
- [ ] Re-do any past-exam questions from Days 1–4 that you got wrong or felt slow on
- [ ] If time permits, re-skim Pasquier's tutorial files: `01+IntroductionToPython.py`, `02+SequencesAndCollections.py`, `03+FlowControlAndRepetition.py`, `04+FunctionsAndLambdaExpressions.py`, `07+HigherOrderFunctions.py` — in `CMP321/PythonTutorials-MPasquier-2025/`
- [ ] **Hand-write a 1-page formula sheet** (forces recall):
    - `map(f, iter)`, `filter(p, iter)`, `reduce(f, iter, [init])` signatures
    - `zip(*iters)`, `enumerate(iter, start=0)`
    - `*args` (tuple), `**kwargs` (dict), `/` positional-only, `*` keyword-only
    - 3 conditions for a closure (nested · references enclosing data · outer returns inner)
    - LEGB scope rule
    - Mutable default-argument trap → fix with `lst=None`
    - `is` vs `==` · `.sort()` returns `None` (use `sorted()` for new list)

#### Day 6 — Fri May 1 · Light Review Only (buffer)

- [ ] No new questions. Re-read formula sheet aloud.
- [ ] Skim any past-exam answers that surprised you on Days 1–5.
- [ ] Set up Respondus Monitor early — don't wait until Sat afternoon.
- [ ] Sleep well.

#### Sat May 2 · 🎯 EXAM 2:30–3:30 PM

- [ ] Be online and set up by **2:20 PM**.
- [ ] Reduced number of questions — read every question carefully before answering.

---

### 🗂 Filtered Table of Contents — Midterm 2 Relevant Questions

> ✅ fully relevant · ⚠️ partially relevant (sub-parts noted) · ❌ skip (out of scope this semester)
>
> **OOP rule of thumb**: skip **every** class / `__init__` / inheritance / abstract / exception question. Tutorials 5 & 6 were not formally covered → all OOP/exception material is ❌.

#### Exam 1: Final Exam (A) — 4 of 9 relevant for M2

| #   | Question                                | Status | Notes                                            |
| --- | --------------------------------------- | ------ | ------------------------------------------------ |
| Q4  | Python Strings & Slicing                | ✅      | C1: raw strings, complex `j+2j`, slicing         |
| Q5  | Python Data Structures                  | ✅      | C2: dicts, sets, swap/unpack                     |
| Q6  | Python Functions & Recursion            | ✅      | C4: recursive minmax, docstrings                 |
| Q8  | Functional Programming (map/filter/red) | ✅      | C7                                               |
| Q9  | Lazy Data Structures & Iterators        | ❌      | Pasquier 08 not covered                          |

#### Exam 2: Midterm 1 (A) — 1 of 5 relevant for M2

| #   | Question                            | Status | Notes                                                              |
| --- | ----------------------------------- | ------ | ------------------------------------------------------------------ |
| Q5  | Python Expressions & Slicing        | ✅      | C1: `x,y=[1,2j]` unpacking, complex, dynamic typing, slicing       |

#### Exam 3: Midterm 2 (A) — 4–5 of 5 relevant

| #   | Question                                          | Status | Notes                                                       |
| --- | ------------------------------------------------- | ------ | ----------------------------------------------------------- |
| Q1  | Python Expressions & Scripting                    | ⚠️     | C2/C3 expressions — useful warm-up                          |
| Q2  | Boolean Expressions & Zip                         | ✅      | C3                                                          |
| Q3  | Functions: Multiple Returns, Overloading & `len`  | ✅      | C4                                                          |
| Q4  | OOP: Class Design & Inheritance                   | ❌      | OOP not in scope                                            |
| Q5  | Functional Programming & Higher-Order Functions   | ✅      | C5/C7                                                       |

#### Exam 4: Midterm 1 (B) — 2 of 4 relevant for M2

| #   | Question                              | Status | Notes                                                                               |
| --- | ------------------------------------- | ------ | ----------------------------------------------------------------------------------- |
| Q1  | Python Expressions & Function Calls   | ✅      | mixed: (a) `len(str(x).split('.')[-1])` C4 · (b) C1/C2 expressions · (c) `range()` C3 |
| Q2  | Python Strings, Tuples & Dictionaries | ✅      | (a) palindrome/duplicates · (b) dict grouping — both C2                             |

#### Exam 5: Final Exam (B) — 3 of 9 relevant for M2

| #   | Question                                  | Status | Notes                                              |
| --- | ----------------------------------------- | ------ | -------------------------------------------------- |
| Q2  | Raw Strings, Assignment & Slicing         | ✅      | C1: raw strings, `x='y'` Python vs C++, slicing    |
| Q3  | Recursive minmax & Fibonacci via reduce   | ✅      | (a) recursive minmax C4 · (b) Fibonacci reduce C7  |
| Q4  | OOP: Docstrings & Comparable              | ❌      | OOP not in scope (docstrings already covered in C4) |
| Q5  | Python Expressions & Slicing              | ✅      | C1: duplicate of E2 Q5                             |
| Q6  | Reversed: Slicing/Iterator/Generator      | ❌      | Iterators not in scope                             |

#### Exam 6: Midterm 2 (B) — 2.5 of 3 relevant

| #   | Question                                          | Status | Notes                                                                 |
| --- | ------------------------------------------------- | ------ | --------------------------------------------------------------------- |
| Q1  | OOP: Abstract Classes & Comparison Operators      | ❌      | OOP not in scope                                                       |
| Q2  | Functional Programming, Closures & Expressions    | ✅      | C4/C5                                                                 |
| Q3  | Higher-Order Functions: reduce & map              | ✅      | C5/C7                                                                 |

#### Exam 7: Midterm 2 (C) — ✅ ALL 5 relevant — highest-value exam

| #   | Question                                       | Status | Notes                                  |
| --- | ---------------------------------------------- | ------ | -------------------------------------- |
| Q1  | Python Expressions & Uniqueness                | ✅      | C2 — sets for uniqueness               |
| Q2  | Python Expressions & Dictionary Grouping       | ✅      | C2                                     |
| Q3  | Comparisons (== vs is) & Pythonic Code         | ✅      | C2/C3                                  |
| Q4  | Function Parameters, F-Strings & Closures      | ✅      | C4                                     |
| Q5  | Higher-Order Patterns & Expressions            | ✅      | C5/C7                                  |

#### Exam 8: Midterm 1 — Spring 2020 (Online) — 3 of 6 relevant for M2

| #   | Question                                                | Status | Notes                                                                   |
| --- | ------------------------------------------------------- | ------ | ----------------------------------------------------------------------- |
| Q2  | Dynamic Typing, Type Inference & Python Expressions     | ✅      | C1                                                                      |
| Q3  | List Replacement, Shadowing, Closures & Lambdas         | ✅      | (a) list slicing replacement C2 · (b) built-in shadowing C4 · (c–d) closures/lambdas C4 |
| Q4  | Square Class & Multiple Inheritance                     | ❌      | OOP not in scope                                                        |
| Q5  | Expressions, Comprehensions & Higher-Order Concepts     | ⚠️     | HOF parts ✅ · skip the "use a comprehension" sub-parts                  |
| Q6  | Iterators, Flatten & Accumulate                         | ❌      | Iterators not in scope                                                  |

#### Exam 9: Midterm 1 — Spring 2021 (Online) — 3 of 4 relevant for M2

| #   | Question                                                                                  | Status | Notes                                                       |
| --- | ----------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------- |
| Q1  | Slicing, Reasons for Studying PLs, Case Sensitivity, Orthogonality & Compilation          | ⚠️     | only the slicing sub-part C1 (rest is M1)                   |
| Q2  | Dynamic Typing, Python Expressions, Slicing & Format                                      | ✅      | C1: dynamic typing, slicing, `.format()` with `divmod`      |
| Q3  | mix() Function, Closures, Lambdas & Sorting                                               | ✅      | C4                                                          |
| Q4  | Square Class & Default Width                                                              | ❌      | OOP not in scope                                            |

#### Exam 10: Midterm 1 — Fall 2021 — 3 of 6 relevant for M2

| #   | Question                                       | Status | Notes                                                       |
| --- | ---------------------------------------------- | ------ | ----------------------------------------------------------- |
| Q2  | String Slicing & Dictionary Comprehension      | ⚠️     | (a) string slicing C1 ✅ · (b) dict comprehension ❌          |
| Q3  | Multiple Returns, Dict Dispatch & Closures     | ✅      | C4                                                          |
| Q4  | Count Class & Diamond Problem                  | ❌      | OOP not in scope                                            |
| Q5  | Higher-Order Expressions & Patterns            | ✅      | C7                                                          |
| Q6  | Generators & StopIteration                     | ❌      | Iterators not in scope                                      |

#### Exam 11: Midterm 1 — Spring 2022 — 3 of 5 relevant for M2

| #   | Question                                              | Status | Notes                                                                                          |
| --- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------- |
| Q2  | lsub Function, auto vs x=1 & pprint                   | ✅      | (a) `lsub` list slicing replacement C2 · (b) `auto` vs `x=1` C1 · (c) `pprint` with f-strings C4 |
| Q3  | Multiple Returns, `__call__`, Sorting & Closures      | ✅      | C4                                                                                             |
| Q4  | Square Class, Default Width & Subclass                | ❌      | OOP not in scope                                                                               |
| Q5  | Higher-Order Patterns, Expressions & reduce           | ✅      | C7                                                                                             |

#### Exam 16: Midterm 1 — Spring 2019 — 4 of 6 relevant for M2

| #   | Question                                              | Status | Notes                                                                          |
| --- | ----------------------------------------------------- | ------ | ------------------------------------------------------------------------------ |
| Q2  | Dynamic Typing, Unique Expressions, Slicing & Format  | ✅      | C1: duplicate of E8 Q2 / E9 Q2                                                 |
| Q3  | lsub Function & Square Class                          | ⚠️     | (a) `lsub` ✅ · (b) Square ❌                                                   |
| Q4  | Average Length & Sieve Comprehension                  | ❌      | only relevant sub-part was the sieve comprehension — out of scope              |
| Q5  | Tail-Recursive lzip, map-based zip & Efficiency       | ✅      | C4/C7                                                                          |
| Q6  | Multiple Choice (Abstraction, Features, Type Check, MI)| ⚠️     | only **MCQ #3** (`type(s) is not str`) C1/C4 ✅ · #1 M1 · #2 mixed M1 · #4 OOP ❌ |

#### Exam 17: Final Exam — Spring 2021 — 2 of 8 relevant for M2

| #   | Question                                              | Status | Notes                                       |
| --- | ----------------------------------------------------- | ------ | ------------------------------------------- |
| Q2  | Templates, range() & Memoized Fibonacci               | ⚠️     | (b) `range()` ✅ · (c) memoised Fibonacci ✅  |
| Q3  | Comprehension/HOF Rewrite & Fibonacci via reduce      | ⚠️     | only (ii) "classic HOFs" rewrite ✅ + (b) Fibonacci reduce ✅ · skip (i) comprehension rewrite |
| Q4  | Reversed: Slicing, Iterator & Generator               | ❌      | Iterators not in scope                      |
| Q5  | Regular Expressions                                   | ❌      | Regex not in scope                          |

> [!note] Exams not listed above (Exam 12, 13, 14, 15) are pure grammar / lexical-analysis / Ch1–Ch3 territory — skip for Midterm 2 prep.

---

## Table of Contents

- [[#Exam 1: Final Exam (A)|Exam 1: Final Exam (A)]]
    - [[#Exam 1: Question 1 — Comment Syntax & Language Costs|Question 1 — Comment Syntax & Language Costs]]
    - [[#Exam 1: Question 2 — BNF Grammar & Parse Trees|Question 2 — BNF Grammar & Parse Trees]]
    - [[#Exam 1: Question 3 — Attribute Grammars (XⁿYⁿZⁿ)|Question 3 — Attribute Grammars (XⁿYⁿZⁿ)]]
    - [[#Exam 1: Question 4 — Python Strings & Slicing|Question 4 — Python Strings & Slicing]]
    - [[#Exam 1: Question 5 — Python Data Structures|Question 5 — Python Data Structures]]
    - [[#Exam 1: Question 6 — Python Functions & Recursion|Question 6 — Python Functions & Recursion]]
    - [[#Exam 1: Question 7 — OOP: Diamond Problem & Interfaces|Question 7 — OOP: Diamond Problem & Interfaces]]
    - [[#Exam 1: Question 8 — Functional Programming (map/filter/reduce)|Question 8 — Functional Programming (map/filter/reduce)]]
    - [[#Exam 1: Question 9 — Lazy Data Structures & Iterators|Question 9 — Lazy Data Structures & Iterators]]
- [[#Exam 2: Midterm 1 (A)|Exam 2: Midterm 1 (A)]]
    - [[#Exam 2: Question 1 — Case Sensitivity & Language Design|Question 1 — Case Sensitivity & Language Design]]
    - [[#Exam 2: Question 2 — Garbage Collection & Compilation|Question 2 — Garbage Collection & Compilation]]
    - [[#Exam 2: Question 3 — BNF, EBNF, Derivations & Ambiguity|Question 3 — BNF, EBNF, Derivations & Ambiguity]]
    - [[#Exam 2: Question 4 — Denotational Semantics (Boolean Expressions)|Question 4 — Denotational Semantics (Boolean Expressions)]]
    - [[#Exam 2: Question 5 — Python Expressions & Slicing|Question 5 — Python Expressions & Slicing]]
- [[#Exam 3: Midterm 2 (A)|Exam 3: Midterm 2 (A)]]
    - [[#Exam 3: Question 1 — Python Expressions & Scripting|Question 1 — Python Expressions & Scripting]]
    - [[#Exam 3: Question 2 — Boolean Expressions & Zip|Question 2 — Boolean Expressions & Zip]]
    - [[#Exam 3: Question 3 — Functions: Multiple Returns, Overloading & `len`|Question 3 — Functions: Multiple Returns, Overloading & `len`]]
    - [[#Exam 3: Question 4 — OOP: Class Design & Inheritance|Question 4 — OOP: Class Design & Inheritance]]
    - [[#Exam 3: Question 5 — Functional Programming & Higher-Order Functions|Question 5 — Functional Programming & Higher-Order Functions]]
- [[#Exam 4: Midterm 1 (B)|Exam 4: Midterm 1 (B)]]
    - [[#Exam 4: Question 1 — Python Expressions & Function Calls|Question 1 — Python Expressions & Function Calls]]
    - [[#Exam 4: Question 2 — Python Strings, Tuples & Dictionaries|Question 2 — Python Strings, Tuples & Dictionaries]]
    - [[#Exam 4: Question 3 — Iterators & Generators|Question 3 — Iterators & Generators]]
    - [[#Exam 4: Question 4 — BNF Grammars & Derivations|Question 4 — BNF Grammars & Derivations]]
- [[#Exam 5: Final Exam (B) — 11 Pages|Exam 5: Final Exam (B) — 11 Pages]]
    - [[#Exam 5: Question 1 — Floor Division & Language Costs|Question 1 — Floor Division & Language Costs]]
    - [[#Exam 5: Question 2 — Raw Strings, Assignment & Slicing|Question 2 — Raw Strings, Assignment & Slicing]]
    - [[#Exam 5: Question 3 — Recursive minmax & Fibonacci via reduce|Question 3 — Recursive minmax & Fibonacci via reduce]]
    - [[#Exam 5: Question 4 — OOP: Docstrings & Comparable Interface|Question 4 — OOP: Docstrings & Comparable Interface]]
    - [[#Exam 5: Question 5 — Python Expressions & Slicing|Question 5 — Python Expressions & Slicing]]
    - [[#Exam 5: Question 6 — Reversed: Slicing vs Iterator vs Generator|Question 6 — Reversed: Slicing vs Iterator vs Generator]]
    - [[#Exam 5: Question 7 — Regular Expressions|Question 7 — Regular Expressions]]
    - [[#Exam 5: Question 8 — BNF Grammar & Parse Trees|Question 8 — BNF Grammar & Parse Trees]]
    - [[#Exam 5: Question 9 — Attribute Grammars (Fortran I Strings)|Question 9 — Attribute Grammars (Fortran I Strings)]]
- [[#Exam 6: Midterm 2 (B)|Exam 6: Midterm 2 (B)]]
    - [[#Exam 6: Question 1 — OOP: Abstract Classes & Comparison Operators|Question 1 — OOP: Abstract Classes & Comparison Operators]]
    - [[#Exam 6: Question 2 — Functional Programming, Closures & Expressions|Question 2 — Functional Programming, Closures & Expressions]]
    - [[#Exam 6: Question 3 — Higher-Order Functions: reduce & map|Question 3 — Higher-Order Functions: reduce & map]]
- [[#Exam 7: Midterm 2 (C)|Exam 7: Midterm 2 (C)]]
    - [[#Exam 7: Question 1 — Python Expressions & Uniqueness|Question 1 — Python Expressions & Uniqueness]]
    - [[#Exam 7: Question 2 — Python Expressions & Dictionary Grouping|Question 2 — Python Expressions & Dictionary Grouping]]
    - [[#Exam 7: Question 3 — Comparisons (== vs is) & Pythonic Code|Question 3 — Comparisons (== vs is) & Pythonic Code]]
    - [[#Exam 7: Question 4 — Function Parameters, F-Strings & Closures|Question 4 — Function Parameters, F-Strings & Closures]]
    - [[#Exam 7: Question 5 — Higher-Order Patterns & Expressions|Question 5 — Higher-Order Patterns & Expressions]]
- [[#Exam 8: Midterm 1 — Spring 2020 (Online)|Exam 8: Midterm 1 — Spring 2020 (Online)]]
    - [[#Exam 8: Question 1 — Language Features, Popularity & Orthogonality|Question 1 — Language Features, Popularity & Orthogonality 🔁]]
    - [[#Exam 8: Question 2 — Dynamic Typing, Type Inference & Python Expressions|Question 2 — Dynamic Typing, Type Inference & Python Expressions 🔁]]
    - [[#Exam 8: Question 3 — List Replacement, Built-in Shadowing, Closures & Lambdas|Question 3 — List Replacement, Built-in Shadowing, Closures & Lambdas 🔁]]
    - [[#Exam 8: Question 4 — Square Class & Multiple Inheritance|Question 4 — Square Class & Multiple Inheritance 🔁]]
    - [[#Exam 8: Question 5 — Expressions, Comprehensions & Higher-Order Concepts|Question 5 — Expressions, Comprehensions & Higher-Order Concepts 🔁]]
    - [[#Exam 8: Question 6 — Iterators, Flatten & Accumulate|Question 6 — Iterators, Flatten & Accumulate 🔁]]
- [[#Exam 9: Midterm 1 — Spring 2021 (Online)|Exam 9: Midterm 1 — Spring 2021 (Online)]]
    - [[#Exam 9: Question 1 — Slicing, Reasons for Studying PLs, Case Sensitivity, Orthogonality & Compilation|Question 1 — Slicing, Reasons for Studying PLs, Case Sensitivity, Orthogonality & Compilation 🔁]]
    - [[#Exam 9: Question 2 — Dynamic Typing, Python Expressions, Slicing & Format|Question 2 — Dynamic Typing, Python Expressions, Slicing & Format 🔁]]
    - [[#Exam 9: Question 3 — mix() Function, Closures, Lambdas & Sorting|Question 3 — mix() Function, Closures, Lambdas & Sorting 🔁]]
    - [[#Exam 9: Question 4 — Square Class & Default Width|Question 4 — Square Class & Default Width 🔁]]
- [[#Exam 10: Midterm 1 — Fall 2021|Exam 10: Midterm 1 — Fall 2021]]
    - [[#Exam 10: Question 1 — Orthogonality (C++ vs Python)|Question 1 — Orthogonality (C++ vs Python) 🔁]]
    - [[#Exam 10: Question 2 — String Slicing & Dictionary Comprehension|Question 2 — String Slicing & Dictionary Comprehension 🔁]]
    - [[#Exam 10: Question 3 — Multiple Returns, Dictionary Dispatch & Closures|Question 3 — Multiple Returns, Dictionary Dispatch & Closures 🔁]]
    - [[#Exam 10: Question 4 — Count Class & Diamond Problem|Question 4 — Count Class & Diamond Problem 🔁]]
    - [[#Exam 10: Question 5 — Higher-Order Expressions & Patterns|Question 5 — Higher-Order Expressions & Patterns 🔁]]
    - [[#Exam 10: Question 6 — Generators & StopIteration|Question 6 — Generators & StopIteration 🔁]]
- [[#Exam 11: Midterm 1 — Spring 2022|Exam 11: Midterm 1 — Spring 2022]]
    - [[#Exam 11: Question 1 — C vs Python & Orthogonality|Question 1 — C vs Python & Orthogonality 🔁]]
    - [[#Exam 11: Question 2 — lsub Function, auto vs x=1 & pprint|Question 2 — lsub Function, auto vs x=1 & pprint 🔁]]
    - [[#Exam 11: Question 3 — Multiple Returns, **call**, Sorting & Closures|Question 3 — Multiple Returns, **call**, Sorting & Closures 🔁]]
    - [[#Exam 11: Question 4 — Square Class, Default Width & Subclass|Question 4 — Square Class, Default Width & Subclass 🔁]]
    - [[#Exam 11: Question 5 — Higher-Order Patterns, Expressions & reduce|Question 5 — Higher-Order Patterns, Expressions & reduce 🔁]]


- [[#Exam 12: Final A — May 2020|Exam 12: Final A — May 2020]]
    - [[#Exam 12: Question 1 — Readability, Writability, Reliability & Cost Criteria|Question 1 — Readability, Writability, Reliability & Cost Criteria]]
    - [[#Exam 12: Question 2 — Parallel Assignment|Question 2 — Parallel Assignment]]
    - [[#Exam 12: Question 5 — Ambiguous Grammars & Parse Trees|Question 5 — Ambiguous Grammars & Parse Trees]]
    - [[#Exam 12: Question 6 — Static vs Dynamic Semantics & Denotational Semantics|Question 6 — Static vs Dynamic Semantics & Denotational Semantics]]
    - [[#Exam 12: Question 7 — Lexical Analysis & Recursive Descent Parsing|Question 7 — Lexical Analysis & Recursive Descent Parsing]]
- [[#Exam 13: Final B — Unknown Semester (Grammar-Heavy)|Exam 13: Final B — Unknown Semester (Grammar-Heavy)]]
    - [[#Exam 13: Question 1 — Hexadecimal BNF Grammar|Question 1 — Hexadecimal BNF Grammar]]
    - [[#Exam 13: Question 2 — BNF Derivation & Proof|Question 2 — BNF Derivation & Proof]]
    - [[#Exam 13: Question 3 — Static vs Dynamic Semantics & Ternary Numbers|Question 3 — Static vs Dynamic Semantics & Ternary Numbers]]
    - [[#Exam 13: Question 4 — Fortran I String Attribute Grammar|Question 4 — Fortran I String Attribute Grammar]]
    - [[#Exam 13: Question 6 — C++ Tokenization|Question 6 — C++ Tokenization]]
- [[#Exam 14: Final C — Unknown Semester (BNF & Attribute Grammars)|Exam 14: Final C — Unknown Semester (BNF & Attribute Grammars)]]
    - [[#Exam 14: Question 2 — C++ Assignments BNF & Switch EBNF|Question 2 — C++ Assignments BNF & Switch EBNF]]
    - [[#Exam 14: Question 3 — Postfix Expressions & Ambiguity|Question 3 — Postfix Expressions & Ambiguity]]
    - [[#Exam 14: Question 4 — English Grammar Ambiguity|Question 4 — English Grammar Ambiguity]]
    - [[#Exam 14: Question 5 — BNF to EBNF|Question 5 — BNF to EBNF]]
    - [[#Exam 14: Question 6 — Roman Numeral Attribute Grammar|Question 6 — Roman Numeral Attribute Grammar]]
- [[#Exam 15: Appendix — Reconstructed Questions|Exam 15: Appendix — Reconstructed Questions]]
    - [[#Exam 15: Palindrome BNF & Attribute Grammar|Palindrome BNF & Attribute Grammar]]
    - [[#Exam 15: Lexical Analyzer vs Parser|Lexical Analyzer vs Parser]]

- [[#Exam 16: Midterm 1 — Spring 2019|Exam 16: Midterm 1 — Spring 2019]]
    - [[#Exam 16: Question 1 — C vs Python RWR, Type Inference Costs & Orthogonality|Question 1 — C vs Python RWR, Type Inference Costs & Orthogonality]]
    - [[#Exam 16: Question 2 — Dynamic Typing, Unique Expressions, Slicing & Format|Question 2 — Dynamic Typing, Unique Expressions, Slicing & Format]]
    - [[#Exam 16: Question 3 — lsub Function & Square Class|Question 3 — lsub Function & Square Class]]
    - [[#Exam 16: Question 4 — Average Length & Sieve Comprehension|Question 4 — Average Length & Sieve Comprehension]]
    - [[#Exam 16: Question 5 — Tail-Recursive lzip, map-based zip & Efficiency|Question 5 — Tail-Recursive lzip, map-based zip & Efficiency]]
    - [[#Exam 16: Question 6 — Multiple Choice (Abstraction, Features, Type Check, MI)|Question 6 — Multiple Choice (Abstraction, Features, Type Check, MI)]]
- [[#Exam 17: Final Exam — Spring 2021|Exam 17: Final Exam — Spring 2021]]
    - [[#Exam 17: Question 1 — Increment Operators & Orthogonality Benefits/Drawbacks|Question 1 — Increment Operators & Orthogonality Benefits/Drawbacks]]
    - [[#Exam 17: Question 2 — Templates, range() & Memoized Fibonacci|Question 2 — Templates, range() & Memoized Fibonacci]]
    - [[#Exam 17: Question 3 — Comprehension/HOF Rewrite & Fibonacci via reduce|Question 3 — Comprehension/HOF Rewrite & Fibonacci via reduce]]
    - [[#Exam 17: Question 4 — Reversed: Slicing, Iterator & Generator|Question 4 — Reversed: Slicing, Iterator & Generator]]
    - [[#Exam 17: Question 5 — Regular Expressions|Question 5 — Regular Expressions]]
    - [[#Exam 17: Question 6 — Ambiguous C++ Grammar & Resolution|Question 6 — Ambiguous C++ Grammar & Resolution]]
    - [[#Exam 17: Question 7 — Palindrome BNF & Attribute Grammar|Question 7 — Palindrome BNF & Attribute Grammar]]
    - [[#Exam 17: Question 8 — Lexical Analyzer vs Syntax Analyzer|Question 8 — Lexical Analyzer vs Syntax Analyzer]]

---

## Midterm 1 — Filtered Table of Contents
> [!open]-
> 
> > **Scope:** Ch1 (Readability/Writability/Reliability/Cost, Orthogonality, Compilation) · Ch3 (BNF/EBNF, Derivations, Parse Trees, Ambiguity, Attribute Grammars, Semantics) · Python Basics (Dynamic Typing, Type Inference, Variables/References, Numbers, Strings, Slicing, Formatting, Raw Strings, Basic Functions, range())
> > 
> > ✅ = Fully in M1 scope · ⚠️ = Partially in scope (sub-parts noted) · ❌ = Not M1 (omitted)
> 
> Make sure to understand this:
> https://claude.ai/public/artifacts/af6d3b3d-eae7-4c09-ab1d-fcfde3efa2fd
> 
> ### Exam 1: Final Exam (A) — 4 of 9 questions relevant
> 
> | #   | Question                          | Status | Notes                                                                     |
> | --- | --------------------------------- | ------ | ------------------------------------------------------------------------- |
> | Q1  | Comment Syntax & Language Costs   | ✅      | Ch1: readability/writability/reliability of comments; cost trends         |
> | Q2  | BNF Grammar & Parse Trees         | ✅      | Ch3: parse trees, proving invalidity, ambiguity                           |
> | Q3  | Attribute Grammars (XⁿYⁿZⁿ)       | ✅      | Ch3: attributes, semantic rules, predicates, decorated parse tree         |
> | Q4  | Python Strings & Slicing          | ✅      | W7: raw strings, complex numbers (`j+2j`), slicing, list slice assignment |
> | Q5  | Python Data Structures            | ⚠️     | (a) swap/unpacking ✅ · (b–c) dicts/sets go beyond W7                      |
> | Q6  | Python Functions & Recursion      | ❌      | Recursive minmax, docstrings — beyond basics                              |
> | Q7  | OOP: Diamond Problem & Interfaces | ❌      |                                                                           |
> | Q8  | Functional Programming            | ❌      |                                                                           |
> | Q9  | Lazy Data Structures & Iterators  | ❌      |                                                                           |
> 
> ### Exam 2: Midterm 1 (A) — ✅ ALL 5 questions relevant
> 
> |#|Question|Status|Notes|
> |---|---|---|---|
> |Q1|Case Sensitivity & Language Design|✅|Ch1: readability/writability/reliability; Python vs C++ containers|
> |Q2|Garbage Collection & Compilation|✅|Ch1: GC effects on all costs; Java compilation steps|
> |Q3|BNF, EBNF, Derivations & Ambiguity|✅|Ch3: nested lists grammar, EBNF conversion, derivation, ambiguity proof|
> |Q4|Denotational Semantics (Boolean)|✅|Ch3: Mₑ rules for Boolean operators, step-by-step evaluation|
> |Q5|Python Expressions & Slicing|✅|W7: `x,y=[1,2j]` unpacking, complex, dynamic typing, slicing|
> 
> ### Exam 3: Midterm 2 (A) — ❌ None relevant
> 
> ### Exam 4: Midterm 1 (B) — 2 of 4 questions relevant
> 
> | #   | Question                              | Status | Notes                                                                              |
> | --- | ------------------------------------- | ------ | ---------------------------------------------------------------------------------- |
> | Q1  | Python Expressions & Function Calls   | ✅      | W7: `len(str(x).split('.')[-1])`, complex (`1+7j`), `range()`, list repetition     |
> | Q2  | Python Strings, Tuples & Dictionaries | ⚠️     | (a) palindrome/duplicates/printing — stretches beyond W7 · (b) grouping function ❌ |
> | Q3  | Iterators & Generators                | ❌      |                                                                                    |
> | Q4  | BNF Grammars & Derivations            | ✅      | Ch3: `0⟨S⟩1 \| 01` interpretation, leftmost derivation, reverse derivation         |
> 
> ### Exam 5: Final Exam (B) — 5 of 9 questions relevant
> 
> |#|Question|Status|Notes|
> |---|---|---|---|
> |Q1|Floor Division & Language Costs|✅|Ch1: `x//y` vs `Math.floor()` vs `int()` — readability/writability/reliability; cost trends|
> |Q2|Raw Strings, Assignment & Slicing|✅|W7: raw strings, `x='y'` Python vs C++, slicing expressions|
> |Q3|Recursive minmax & Fibonacci reduce|❌||
> |Q4|OOP: Docstrings & Comparable|❌||
> |Q5|Python Expressions & Slicing|✅|Same as Exam 2 Q5 (duplicate)|
> |Q6|Reversed: Slicing vs Iterator vs Generator|❌||
> |Q7|Regular Expressions|❌||
> |Q8|BNF Grammar & Parse Trees|✅|Same grammar as Exam 1 Q2 (duplicate)|
> |Q9|Attribute Grammars (Fortran I Strings)|✅|Ch3: attributes, predicates, semantic rules, decorated parse tree|
> 
> ### Exam 6: Midterm 2 (B) — ❌ None relevant
> 
> ### Exam 7: Midterm 2 (C) — ❌ None relevant
> 
> ### Exam 8: Midterm 1 — Spring 2020 (Online) — 2.5 of 6 questions relevant
> 
> > ⚠️ COVID-era online exam — covers full semester, not just M1 material
> 
> |#|Question|Status|Notes|
> |---|---|---|---|
> |Q1|Language Features, Popularity & Orthogonality|✅|Ch1: reasons for studying PLs, C vs Python, orthogonality (Java types, C++ semicolon)|
> |Q2|Dynamic Typing, Type Inference & Python Expressions|✅|W7: dynamic typing, `auto x=1` vs `x=1`, unique expressions, slicing|
> |Q3|List Replacement, Shadowing, Closures & Lambdas|⚠️|(a) list slicing replacement ✅ · (b) built-in shadowing ✅ · (c–d) closures/lambdas ❌|
> |Q4|Square Class & Multiple Inheritance|❌||
> |Q5|Expressions, Comprehensions & Higher-Order|❌||
> |Q6|Iterators, Flatten & Accumulate|❌||
> 
> ### Exam 9: Midterm 1 — Spring 2021 (Online) — 2 of 4 questions relevant
> 
> > ⚠️ COVID-era online exam — covers more than standard M1
> 
> |#|Question|Status|Notes|
> |---|---|---|---|
> |Q1|Slicing, Reasons, Case Sensitivity, Orthogonality & Compilation|✅|Ch1+W7: slicing, reasons for studying PLs, case sensitivity, orthogonality, compilation steps|
> |Q2|Dynamic Typing, Python Expressions, Slicing & Format|✅|W7: dynamic typing, unique expressions, slicing, `.format()` with `divmod`|
> |Q3|mix() Function, Closures, Lambdas & Sorting|❌|All sub-parts require closures/lambdas/sorting beyond W7|
> |Q4|Square Class & Default Width|❌||
> 
> ### Exam 10: Midterm 1 — Fall 2021 — 1.5 of 6 questions relevant
> 
> > ⚠️ Covers far more than standard M1 — likely combined/cumulative
> 
> |#|Question|Status|Notes|
> |---|---|---|---|
> |Q1|Orthogonality (C++ vs Python)|✅|Ch1: pass-by-value vs reference, orthogonality definition|
> |Q2|String Slicing & Dictionary Comprehension|⚠️|(a) slicing ✅ · (b) dict comprehension ❌|
> |Q3|Multiple Returns, Dict Dispatch & Closures|❌|All sub-parts beyond W7|
> |Q4|Count Class & Diamond Problem|❌||
> |Q5|Higher-Order Expressions & Patterns|❌||
> |Q6|Generators & StopIteration|❌||
> 
> ### Exam 11: Midterm 1 — Spring 2022 — 1.5 of 5 questions relevant
> 
> > ⚠️ Another combined exam — most content is M2-level
> 
> |#|Question|Status|Notes|
> |---|---|---|---|
> |Q1|C vs Python & Orthogonality|✅|Ch1: readability/writability/reliability comparison, orthogonality via assignment|
> |Q2|lsub Function, auto vs x=1 & pprint|⚠️|(a) list slicing replacement ✅ · (b) `auto` vs `x=1` type inference ✅ · (c) pprint with f-strings ⚠️|
> |Q3|Multiple Returns, **call**, Sorting & Closures|❌||
> |Q4|Square Class, Default Width & Subclass|❌||
> |Q5|Higher-Order Patterns, Expressions & reduce|❌||
> 
> ## Midterm 1 — Filtered Tables (Exams 12–15)
> 
> ### Exam 12: Final A — May 2020 — 5 of 7 questions relevant
> 
> |#|Question|Status|Notes|
> |---|---|---|---|
> |Q1|Readability, Writability, Reliability & Costs|✅|Ch1: `A && !B` vs `A and not B`, `count=1` vs `int count=1`; pointer costs|
> |Q2|Parallel Assignment, Stack, Fib, FuncPool, Bug|⚠️|(a) `a,b=b,a` ✅ 🔁 Exam 1 Q5(a) · (b–e) stack/fib/funcpool/type bug ❌|
> |Q3|Reversed Iteration: Slicing, Iterator, Generator|❌||
> |Q4|BNF to Regex: Email Addresses|❌|Regex = Week 13|
> |Q5|Ambiguous Grammars & Parse Trees|✅|Ch3: ambiguity, parse trees, proof, unambiguous rewrite, BNF/EBNF/Attr Grammar for adjectives|
> |Q6|Static vs Dynamic Semantics & Denotational|✅|Ch3: static vs dynamic semantics; denotational semantics Boolean eval 🔁 Exam 2 Q4|
> |Q7|Lexical Analysis & Recursive Descent Parsing|✅|W4: tokenization C++ vs Python, left recursion fix, derivation|
> 
> ### Exam 13: Final B — Unknown Semester — 4.5 of 7 questions relevant
> 
> |#|Question|Status|Notes|
> |---|---|---|---|
> |Q1|Hexadecimal BNF Grammar|✅|Ch3: BNF construction, proving grammar incorrectness|
> |Q2|BNF Derivation & Proof|✅|Ch3: leftmost derivation, prove not in language 🔁 Exam 2 Q3(c-d)|
> |Q3|Static vs Dynamic Semantics & Ternary Numbers|✅|(a) static vs dynamic 🔁 Exam 12 Q6(a) · (b) ternary BNF + semantic rules ✅|
> |Q4|Fortran I String Attribute Grammar|✅|🔁 Exam 5 Q9 — identical question|
> |Q5|(Not captured)|—||
> |Q6|C++ Tokenization, State Diagrams & Regex|⚠️|(a) tokenization ✅ W4 · (b–c) state diagrams/regex ❌|
> |Q7|Regex Descriptions & HTML Tag Correction|❌|Regex = Week 13|
> 
> ### Exam 14: Final C — Unknown Semester — All 5 visible questions relevant
> 
> |#|Question|Status|Notes|
> |---|---|---|---|
> |Q1|(Not captured)|—||
> |Q2|C++ Assignments BNF & Switch EBNF|✅|Ch3: BNF for cascading assignments, EBNF for switch, syntax diagrams|
> |Q3|Postfix Expressions & Ambiguity|✅|Ch3: BNF interpretation, derivation, parse tree, reverse derivation, ambiguity|
> |Q4|English Grammar Ambiguity|✅|Ch3: two parse trees, ambiguity proof, unambiguous rewrite|
> |Q5|BNF to EBNF to Regex & Format Specifiers|⚠️|(a) BNF interpretation + EBNF conversion ✅ · regex part ❌ · (b) regex ❌|
> |Q6|Roman Numeral Attribute Grammar|✅|Ch3: semantic rules, evaluation, predicates, decorated parse tree|
> 
> ### Exam 15: Appendix — Both questions relevant
> 
> |#|Question|Status|Notes|
> |---|---|---|---|
> |A1|Palindrome BNF & Attribute Grammar|✅|Ch3: BNF limitations, attribute grammar with predicates|
> |A2|Lexical Analyzer vs Parser|✅|W4: tokenization, ambiguity between sign and operator|
> 
> ### Exam 16: Midterm 1 — Spring 2019 — 4.5 of 6 questions relevant
> 
> |#|Question|Status|Notes|
> |---|---|---|---|
> |Q1|C vs Python RWR, Type Inference Costs, Orthogonality|✅|(a) 🔁 Exam 8/11 · (b) type inference costs NEW · (c) orthogonality 🔁 Exam 8|
> |Q2|Dynamic Typing, Unique Expressions, Slicing, Format|✅|All 🔁 Exam 8/9|
> |Q3|lsub Function & Square Class|✅|(a) 🔁 Exam 8/11 · (b) 🔁 Exam 8/9/11|
> |Q4|Average Length & Sieve Comprehension|⚠️|(a) avg length 🔁 Exam 6/8/11 · (b) sieve comprehension NEW|
> |Q5|Tail-Recursive lzip, map zip & Efficiency|✅|All NEW — tail recursion, map-based zip, iterator efficiency|
> |Q6|MCQ: Abstraction, Features, Type Check, MI|✅|All NEW — 4 multiple-choice questions|
> 
> ### Exam 17: Final — Spring 2021 — 5.5 of 8 questions relevant
> 
> |#|Question|Status|Notes|
> |---|---|---|---|
> |Q1|Increment Operators & Orthogonality|✅|(a) count=count+1 vs count++ NEW · (b) strict orthogonality benefit/drawback NEW|
> |Q2|Templates, range() & Memoized Fibonacci|✅|(a) why Python no templates NEW · (b) range() NEW · (c) memoized fib NEW|
> |Q3|Comprehension/HOF Rewrite & Fib via reduce|⚠️|(a) for-loop rewrite NEW · (b) Fibonacci reduce 🔁 Exam 5 Q3(b)|
> |Q4|Reversed: Slicing, Iterator & Generator|❌|🔁 Exam 5 Q6|
> |Q5|Regular Expressions|❌|Regex = beyond M1 scope|
> |Q6|Ambiguous C++ Grammar & Resolution|⚠️|(a) ambiguity 🔁 Exam 2 Q3(d) · (b) resolve ambiguity NEW|
> |Q7|Palindrome BNF & Attribute Grammar|✅|🔁 Exam 15 Appendix (but fuller question text here)|
> |Q8|Lexical Analyzer vs Syntax Analyzer|✅|Expanded version of Exam 15 A2 — full grammar rules, 3 tokenization examples, sign ambiguity NEW|
> 
## Exam 1: Final Exam (A)

---

### Exam 1: Question 1 — Comment Syntax & Language Costs

**(a)** Many modern languages, including C++ and Java, allow two types of comments: in one case delimiters are used on _both_ ends (e.g., `/*` and `*/`); in the other, a delimiter marks only the _start_ of the comment (e.g., `//`), which ends with the line. Explain briefly whether each of these is good or bad with respect to the criteria of _readability_, _writability_, and _reliability_ — and why. **(6 marks)**

> **📝 Note:** Answer requires filling in the following table:

Fill in the table:

|                                  | Readability | Writability | Reliability |
| -------------------------------- | ----------- | ----------- | ----------- |
| **Both ends** (e.g. `/* ... */`) |             |             |             |
| **Start only** (e.g. `//`)       |             |             |             |

> [!success]- Solution
> 
> |                                  | Readability                                                                                           | Writability                                                                                                                 | Reliability                                                                                                                                                 |
> | -------------------------------- | ----------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
> | **Both ends** (e.g. `/* ... */`) | Good for long explanations, but the closing */ can be far away so it's hard to see where comments end | Less writability than // because it takes longer and typically involves multi-line comments which can take longer to write. | Forgetting the \*/ silently comments out actual code, and may cause hard-to detect bugs. May accidentally nest comments too /\* /\* \*/ \*/ causes an error |
> | **Start only** (e.g. `//`)       | Clear, since the comment always end at the line, so there's no ambiguity.                             | Quick and easy to write                                                                                                     | reliable since there is no risk of forgetting \*/. Also can handle nesting unlike /*                                                                        |
> 
---

**(b)** Indicate for each of the _costs_ of programming languages below whether it has generally _increased or decreased_ over the last decades, and _why_. **(4 marks)**

- **Training:**
- **Coding:**
- **Tools:**
- **Execution:**
- **Reliability:**

> [!success]- Solution
> **Training**: generally decreased as the barrier to entry for programming languages became easier, moving from complex languages like Fortran to Python, the latter of which mimics natural language more and thus is easier to learn and adopt.
> 
> **Coding**: generally decreased. Now, higher-level languages provide better abstraction and expressivity, including through the use of built-in functions, libraries, garbage collection, etc. which requires less code to write.
> 
> **Tools**: generally decreased. Tools used to be more expensive proprietary software. Now most are free and open-source (VS Code, GCC, Python interpreter). More tools means more free options.
> 
> **Execution**: generally increased. Modern languages are slower than C and Fortran. Hardware got faster, but the languages themselves got slower. This is because older languages were compiled directly to machine code, whereas modern languages may perform type checking, garbage collection, virtual machines, etc. 
> 
> **Reliability**: generally decreased. With time, language developers became more aware of common human errors, bugs, performance drainers, and other issues related to the language, and have created specific error messages, handled some cases, etc. to address it. This meant fewer bugs, less debugging, less maintenance.

---

### Exam 1: Question 2 — BNF Grammar & Parse Trees

Given the following BNF grammar:

```
⟨sentence⟩    → ⟨subject⟩ ⟨predicate⟩
⟨subject⟩     → ⟨article⟩ ⟨noun⟩
⟨predicate⟩   → ⟨verb⟩ ⟨object⟩
⟨object⟩      → ⟨article⟩ ⟨noun⟩

⟨article⟩     → A | AN | THE
⟨noun⟩        → CAT | DOG | MAN
⟨verb⟩        → BITES | PETS
```

**(a)** Using the BNF grammar above, draw a complete parse tree to show that the sentence **THE MAN PETS A DOG** is valid in this language. **(3 marks)**

> [!success]- Solution
> Parse tree:
> ![image-40.png|400x240](/img/user/1%20-%20MW%20CMP321/img/image-40.png)
> Derivation (not asked for):
> 
> ```
> <sentence>
> <subject>        <predicate>
> <article> <noun> <predicate>
> THE       <noun> <predicate>
> THE       MAN    <predicate>
> THE       MAN    <verb> <object>
> THE       MAN    PETS   <object>
> THE       MAN    PETS   <article> <noun>
> THE       MAN    PETS   A         <noun>
> THE       MAN    PETS   A         DOG
> ```

---

**(b)** Prove that the sentence **A DOG BITES PETS** is _not_ in this language. **(4 marks)**

Must start with \<subject> to use rule #1 and get form after recognition.

> [!success]- Solution
> 
> ```
> A DOG BITES PETS
> <article> DOG    BITES    PETS
> <article> <noun> BITES    PETS
> <subject>        BITES    PETS
> <subject>        <verb>   PETS
>     
> <subject>        <verb>   <verb> is not possible. The only closest possible rule to apply for <verb> X is <verb> <object>. Therefore, no valid sentence.
> ```
> 

---

**(c)** Explain briefly how in BNF we could exclude sentences that _are_ actually in the language, but should _not_ be, such as **A MAN BITES THE DOG**. **(3 marks)**

> [!success]- Solution
> Split the grammar into separate categories (e.g., human vs animal subjects/predicates) so that invalid semantic combinations become syntactically impossible
> 
> (optional explanation:)
> ```
> ⟨sentence⟩    → ⟨human_subject⟩ ⟨human_predicate⟩ | <animal_subject> <animal_predicate>
> ⟨human_subject⟩     -> ⟨article⟩ <person>
> ⟨human_predicate⟩   -> PETS ⟨object⟩
> <animal_subject>   -> <article> <noun>
> <animal_predicate> -> BITES <object>
> ⟨object⟩      → ⟨article⟩ ⟨noun⟩
> 
> ⟨article⟩     → A | AN | THE
> <person>     -> MAN
> ⟨noun⟩        → CAT | DOG
> ```

---

**(d)** Is the above grammar _ambiguous_? Justify clearly your answer. **(2 marks)**

> [!success]- Solution
> No.
> - `⟨sentence⟩` has only one rule
> - `⟨subject⟩` has only one rule
> - `⟨predicate⟩` has only one rule
> Every sentence has exactly one way to parse it

---

### Exam 1: Question 3 — Attribute Grammars (XⁿYⁿZⁿ)

The BNF grammar on the right defines sentences comprising one or more X followed by one or more Y and one or more Z. What we really want, however, are sentences with the _same number_ of X, Y, and Z — i.e., of the form XᴺYᴺZᴺ for N>0.

```
⟨S⟩   → ⟨Xs⟩ ⟨Ys⟩ ⟨Zs⟩
⟨Xs⟩  → X | ⟨Xs⟩ X
⟨Ys⟩  → Y | ⟨Ys⟩ Y
⟨Zs⟩  → Z | ⟨Zs⟩ Z
```

**(a)** Extend this grammar accordingly with the necessary _attributes_, _semantic rules_, and _predicates_. Explain your design clearly. **(6 marks)**

> [!success]- Solution
> ```
> Attribute (What do i need to track?):
> 
> count ∈ {1,2,3,...}
> 
> Semantics (How does the value build up?):
> 
> base case
> <Xs> → X         <Xs>.count = 1
> recursive case
> <Xs> → ⟨Xs⟩ X     <Xs>[0].count = <Xs>[1].count + 1
> 
> Predicate (What constraint must hold?):
> <Xs>.count == <Ys>.count
> <Ys>.count == <Zs>.count
> ```
> 
> FYI: count can never be 0 because grammar requires at least one X,Y, and Z.


---

**(b)** Draw the parse tree for the sentence **X²Y³Z²** and _decorate_ it clearly to show all synthesized attributes and their values, assuming none are inherited. Point out exactly _where_ and _how_ a syntax error is discovered. **(4 marks)**

> [!success]- Solution
> ![image-41.png|400x264](/img/user/1%20-%20MW%20CMP321/img/image-41.png)

---

### Exam 1: Question 4 — Python Strings & Slicing

**(a)** What is a _raw string_ in Python and what exactly is its purpose? Explain clearly using an appropriate example of your choosing. **(3 marks)**

> [!success]- Solution
> To print something literally where backslashes are not interpreted as an operation like starting a new line (\n), tab (\t), etc. but instead just plaintext. Therefore: print(r'hi \n everyone') will literally print 'hi \n everyone' whereas print('hi \n everyone') would have resulted in: 
> hi
> everyone
> 
> It is useful for operations like indicating file path: (r'C:\Users\newUser\today_class')


---

**(b)** Explain _how_ the output of the Python expression `print(j+2j)` can be: `4j`. Indicate which objects are created, in order. **(3 marks)**

> [!success]- Solution
> `j` is variable name. It can be defined as 2j.
> 2j is complex number
> 
> If `j` was defined as 2j, 2j (from variable `j`) + 2j (complex number), would result in 4j.
> 
> 1. j variable is created and holds a reference to 2j (object).
> 2. 2j is value of temporary complex number object.
> 3. j and 2j are added and result in creation of new object (4j).
> Therefore, 3 objects are created (2j, 2j, 4j).
> print() is then called.

---

**(c)** Explain in detail what the following Python statement does exactly and what its output is: **(3 marks)**

```python
'Is Halloween important?'[-3::-13]
```


> [!success]- Solution
> string\[start:end:step\]. So in this case the start is -3. end is beginning of array. step is -13.
> go from -3 (third last char) to start of array (reverse movement) and jump 13 chars backwards (skip 12) and print.
> 
> OUTPUT: no

---

**(d)** Indicate what the expression below will do to a given list `lst`. Justify briefly your answer. **(3 marks)**

> [!success]- Solution
> 
> ```python
> lst[::2] = ['_'] * (len(lst) // 2)
> ```
> start: beginning of array
> end: end of array
> step: every 2 elements (0,2,4,...)
> 
> After every 2 elements from beginning till end of list, replace each element with the corresponding value in RHS array. This performs LHS slice assignment.
> 
> `lst[::2] = ['_','_','_']`  (works similar to a,b,c = \[1,2,3\])
> 
> So a list like `[1,2,3,4,5,6]` would be `['_',2,'_',4,'_',6]`. So this works for even lengths, since here the number of slots (3) are equal to number of values (3).
> 
> However, a list like \[1,2,3,4,5,6,7\] won't work, it'll be like `['_',2,'_',4,'_',6,?]`. This doesn't work since the number of slots is 4, whereas number of values is 3. It expects 1 more value.
> 
> ValueError: can't assign 3 items to 4 slots.

---

### Exam 1: Question 5 — Python Data Structures

**(a)** State the _differences_ between the expressions `x,y=[y,x]` and `x,y=y,x` in terms of the objects created, the steps, and/or the result achieved. **(2 marks)**

> [!success]- Solution
> `x,y=y,x`
> 1. Creates a temporary tuple (immutable, lighter)
> 2. Unpacks tuple into x,y , i.e.  x,y=(y,x). Therefore, x points to value of y. y points to value of x.
> Final outcome: 2 objects is left (same as what we started with). x references y value, y references x value. Temporary tuple is garbage collected.
> 
> `x,y=[y,x]`
> This also performs unpacking, but with the addition of creating a list first.
> 1. RHS evaluated first: create a list [y,x] with current value (mutable, heavier)
> 2. Unpacks list into x,y  , i.e. x,y=\[y,x\].
> Final outcome: one temporary list object was made and garbage collected. 2 objects remain (x,y objects)
> 
> Both result in x=y and y=x swaps. However, the means of achieving it differ (tuple vs list).

> [!success]- Alternative Solution
> list unpacking
> tuple unpacking
> 
> They both work the same its just list unpacking is less efficient than tuple unpacking since it requires more memory (since it's mutable, whereas tuple is immutable and thus more optimal for this use case). 
> 
> They both end up swapping the elements of x and y (by simultaneously binding x to reference of object that y was formerly bound to AND y is binded the reference of object that x was formerly bound to SIMULTANEOUSLY.


---

**(b)** Indicate, for each of the statements below about Python dictionaries, whether it is _true or false_, and _why_ exactly. **(6 marks)**

- Dictionary elements are accessed by key.
- Dictionaries are immutable data structures.
- Dictionaries can be nested to any depth.
- Dictionary keys can be anything.

b)

> [!success]- Solution
> TRUE. They are only accessed from a key value and not sequence-based like list, tuples, and strings.
> FALSE. You may replace values of dictionary and add more. For example, if key "james_age" didn't exist in Dictionary dict we can add it like so dict["james_age"]=10
> TRUE. we can have dict["james"]={age:10, year:2016}
> FALSE. keys must be immutable (string, float, int, tuples frozenset), so for example you can't have a list as a key of dictionary.

---

**(c)** State which data structure a Python _set_ uses internally, and _why_. **(2 marks)**

> [!success]- Solution
> uses hash tables internally because it is faster that way (O(1) lookup). This is also why it is unordered. So to look for if a value exists in set it would be quick because it just performs hash function on the value you're looking for and if the result is in the hash table (after all collision checks using \==) then it will return yes.

---

### Exam 1: Question 6 — Python Functions & Recursion

**(a)** Consider the Python code below. Explain briefly but precisely what will happen to each of the two strings, and what the function call will do. **(4 marks)**

```python
def fun():
    "hello, world!"
    "bye for now."
    print(fun)
fun()
```

> [!success]- Solution
> it will say <function fun at 0x...> and wont print anything. "hello, world!" will become docstring accessible via fun.__doc__ and help(fun), whereas "bye for now." will just be executed then garbage collected.

---

**(b)** Write a _recursive_ minmax function in Python that returns _both_ the smallest and largest items from a given iterable. Make sure your code works in _all_ cases, that it is _efficient_ (traversing the iterable only once), and that it fully uses the language features (but not the `min`/`max` functions, of course). **(8 marks)**

> [!success]- Solution
> ![image-55.png|400x383](/img/user/1%20-%20MW%20CMP321/img/image-55.png)
> \*typo: space before "else"

def minmax(seq):
         if not seq:
                 return None, None
        if len (seq) == 1:
                return seq[0], seq [0]
       rest_min, rest_max = minmax(seq[1:]) 

---

### Exam 1: Question 7 — OOP: Diamond Problem & Interfaces

**(a)** Explain what the _diamond problem_ is in object-oriented programming, why it _must_ exist in Python, and _how_ the language solves the issue. **(4 marks)**

---

**(b)** Explain the output of the print statement below, esp. what is compared and why. Define the `Comparable` abstract class that will act as an interface, then modify the `Point` class accordingly to "implement" this interface. Note that the same print statement should now show the correct result. **(6 marks)**

```python
class Point:
    def __init__(self, x=0, y=0): self.x, self.y = x, y
    def __str__(self): return f'[{self.x}, {self.y}]'

print(Point(1,2) == Point(1,2))
```

Write the `Comparable` class and modified `Point(Comparable)` class:

```python
class Comparable(
    '''a Java-like "interface" for comparing objects'''

class Point(Comparable):
    def __init__(self, x=0, y=0): self.x, self.y = x, y
    def __str__(self): return f'[{self.x}, {self.y}]'
    def ...
```

---

### Exam 1: Question 8 — Functional Programming (map/filter/reduce)

**(a)** ⭐ Write a single Python expression, using _only_ `map`/`filter`/`reduce` with appropriate lambda expressions, to retrieve a hidden password by combining the second last letter of each N-letter long word in a given list of strings. **(4 marks)**

**Example:**

```
N=5; words=['mango', 'pear', 'lemon', 'nut', 'cherry',
            'pecan', 'orange', 'apple']   → 'goal'
```

> [!success]- Solution
> ```python
> reduce(lambda a,b: a+b, map(lambda y: y[-2], filter(lambda x: len(x)==N, words)))
> ```

---

**(b)** Rewrite the expression below using _comprehension syntax_ and simplifying as much as possible. Point out where a generator is used, if any. **(3 marks)**

```python
reduce(operator.add, filter(lambda n: n>0, map(float, lst)))
```

---

**(c)** State _which_ well-known Python higher-order function the mystery function below implements. Explain briefly _when_ it is needed and _how_ it works, using a simple example of your choosing. **(5 marks)**

```python
def mystery(function, iterable):
    for it in iterable:
        yield function(*it)
```

> [!success]- Solution
> mystery is the itertools.starmap function. It's needed when you have an iterable of tuples and want to apply a multi-argument function to each tuple's elements as separate positional args. The *it syntax inside the call is what unpacks each tuple. Example: mystery(pow, [(2,3), (4,2), (3,3)]) yields 8, 16, 27. Equivalent to pow(2,3), pow(4,2), pow(3,3)

---

### Exam 1: Question 9 — Lazy Data Structures & Iterators

**(a)** Explain briefly what a _lazy data structure_ is, and indicate _two_ of its key benefits to a programming language. **(3 marks)**

---

**(b)** Answer the following about the `Polygon` class and code below. **(9 marks)**

```python
class Polygon:    # comprises a list of 2D points: (X, Y, NAME)
    def __init__(self, *points): self._pts = points
    def __len__(self): return len(self._pts)
    def __str__(self): return ' '.join(f'{name}({x},{y}) '
                                       for x, y, name in self._pts)

poly = Polygon((0,0,'O'), (1,2,'A'), (3,1,'B'))
```

**(i)** Will the following expression work? Explain exactly why, or not. If needed, modify the class to make it work.

```python
for p in poly._pts: print(p)
```

---

**(ii)** Will the following expression work? Explain exactly why, or not. If needed, modify the class to make it work.

```python
for p in poly: print(p)
```

---

**(iii)** Show (only) the _changes_ to the class needed for the following to work:

```python
for _ in range(5): print(next(poly), end=' ')
#→ (0, 0, 'O') (1, 2, 'A') (3, 1, 'B') None (0, 0, 'O')
```

---

_End of Exam 1_

---

## Exam 2: Midterm 1 (A)

---

### Exam 2: Question 1 — Case Sensitivity & Language Design

**(a)** Modern programming languages distinguish _uppercase_ from _lowercase_ in identifiers (e.g., variable and function names). Elaborate the reasons for this design decision in terms of _readability_, _writability_, and _reliability_. **(6 marks)**

> [!success]- Solution
> - **Readability**: Case sensitivity allows for naming conventions (e.g. MyClass, myVariable) that signal what kind of identifier something is. This improves readability. However, foo and Foo look very similar but are different identifiers. This can confuse readers. Therefore, this has a mixed effect on readability.
> - **Writability**: It increases writability since it's giving increased flexibility to the user by providing more naming options (and thus a larger namespace to work with). You can use x and X as separate identifiers.
> - **Reliability**: This can produce accidental user-induced bugs in terms of accidentally performing an action on x instead of X or vice versa. This is also hard to detect, similar to aliasing, and therefore lowers reliability.

---

**(b)** With reference to programming language characteristics (evaluation criteria), indicate precisely _why_ Python offers _only_ the `list` class as linear container whereas C++ has many e.g., `vector`, `array`, `list`, `fwd_list`... **(3 marks)**

> [!success]- Solution
> Python tends to favor simplification over performance, and thus prefers to have many features in one class as opposed to C++'s method, which is to tailor to specific use cases and optimize accordingly. 
> 
> **Readability**: Python's method increases readability. This is because having one class as opposed to many variations is easier to understand as the main difference between vectors, arrays, etc. are minor functionality/optimization differences but the core goal is the same: containing data.
> **Writeability**: Increases writeability since it lowers the decision overhead, i.e. the time it takes for the developer to decide which container is most appropriate for the data (therefore making it faster to write). Meanwhile, the number of features within the class is not lowered, therefore the flexibility is unaffected. (e.g. slicing, indexing, etc.).
> **Reliability**: Increases reliability since all the features are in one class, the developer does not need to remember which feature applies to which class, and thus decreases risk of accidentally applying a feature to an incompatible class (ex. feature exclusive to dynamically typed on statically typed)
> **Cost**: training cost is lowered (only one container to learn) and writing/coding time is lowered (less time spending changing or thinking about which container to choose), also reduces bug and maintenance costs, but execution cost rises (general-purpose container can't be optimized for every use case like C++) 

---

### Exam 2: Question 2 — Garbage Collection & Compilation

**(a)** Does _garbage collection_ (GC) increase or decrease the various _costs_ of a programming language listed below? _Justify_ briefly your answers. **(6 marks)**

- **Training:**
- **Coding:**
- **Compilation:**
- **Execution:**
- **Tools:**
- **Reliability:**

> [!success]- Solution
> * Training: Decreases training cost as it lowers the time needed to learn how to manually clear unused memory.
> * Coding: Decreases coding cost as it takes less time to write the code (less lines of code and thus time spent coding garbage collection features)
> * Compilation: Decreases compilation cost since it's less code for developer to write (no destructors, delete) so the compiler has fewer lines to process. 
> * Execution: Increases execution cost since garbage collector runs periodically during execution, scanning for unused objects and freeing them. If programmer managed memory manually, it wouldn't have needed to periodically scan (pausing execution to scan all of memory, which happens even there's nothing to free).
> * Tools: Increases tools cost because language creators have to design, implement, and maintain the garbage collector.
> * Reliability: Decreases reliability cost since it will prevent memory leaks, dangling pointers, and double-free bugs, which are among the most common and dangerous errors in C++ and often hard to notice (silent bug). 

---

**(b)** List out all the _steps_ of the compilation process that starts with a Java source code file and ends with a running app. (No need for details.) Indicate which steps are optional, if any. **(3 marks)** ★ 

> [!success]- Solution
> https://claude.ai/public/artifacts/e7b8be29-1c4f-49df-8c0c-6648f825608f
> ![image-8.png|400](/img/user/1%20-%20MW%20CMP321/img/image-8.png)
> Source code (.java)
> Lexical analysis → tokens
> Syntax analysis → parse tree
> Semantic analysis / intermediate code → bytecode (.class)
> Optimization (optional)
> Linking — combine with libraries
> Loading — JVM loads bytecode into memory
> JVM interprets bytecode (or JIT compiles to machine code)
> Execution

---

### Exam 2: Question 3 — BNF, EBNF, Derivations & Ambiguity

**(a)** Describe what data structure the BNF grammar rules below define, and what the format is exactly. Give one example of the simplest possible sentence and one example of a sentence where both recursive cases are applied twice. **(4 marks)**

```
⟨S⟩ → [ ⟨L⟩ ]              ⟨I⟩ → ⟨S⟩ | ⟨N⟩
⟨L⟩ → ⟨I⟩ | ⟨L⟩ , ⟨I⟩      ⟨N⟩ → 1 | 2 | 3 | 4
```

> [!success]- Solution
> ![image-31.png|400x365](/img/user/1%20-%20MW%20CMP321/img/image-31.png)

---

**(b)** Show which rule/s of the grammar in part (a) can be written better in EBNF. Explain accordingly whether EBNF is _useful_, or not, in this case. **(2 marks)**

> [!success]- Solution
> ```
> ⟨S⟩ → '[' ⟨I⟩ {',' ⟨I⟩} ']'
> ⟨I⟩ → ⟨S⟩ | ⟨N⟩
> ⟨N⟩ → 1 | 2 | 3 | 4
> ```
> 
> Yes, because the use of repetition removes the need for \<L> entirely

---

**(c)** Using the BNF grammar below, write a detailed _left-most derivation_ to show that the sentence `'the cat likes to eat and play'` is valid. **(3 marks)**

```
⟨s⟩  → ⟨np⟩ ⟨vp⟩                ⟨d⟩  → a | the | every
⟨np⟩ → ⟨d⟩ ⟨n⟩                  ⟨n⟩  → cat | dog | hamster
⟨vp⟩ → ⟨av⟩ ⟨v⟩                 ⟨av⟩ → can | 'likes to'
⟨vp⟩ → ⟨av⟩ ⟨v⟩ and ⟨v⟩         ⟨v⟩  → eat | play | run
```

> [!success]- Solution
> ![image-32.png|400x274](/img/user/1%20-%20MW%20CMP321/img/image-32.png)

---

**(d)** The BNF grammar rules below define C++ output statements, where `⟨ostream⟩` can be any valid string stream variable (e.g., `cout`), also `⟨string⟩` represents any valid string object, and `⟨int⟩` denotes a literal integer.

```
⟨xpr⟩ → ⟨xpr⟩ '<<' ⟨xpr⟩ | ⟨obj⟩
⟨obj⟩ → ⟨ostream⟩ | ⟨string⟩ | ⟨int⟩
```

**(i)** Explain from principles exactly _why_ this grammar is _ambiguous_. **(3 marks)**

**(ii)** To prove the above, show two different _parse trees_ for the sentence: `cout << "n=" << 8` **(3 marks)**

> [!success]- Solution
> ![image-34.png|400x240](/img/user/1%20-%20MW%20CMP321/img/image-34.png)

---

### Exam 2: Question 4 — Denotational Semantics (Boolean Expressions)

**(a)** Complete the rules of _denotational semantics_ hereafter to define Boolean operators according to the given BNF grammar. **(5 marks)**

```
⟨B⟩ → True
⟨B⟩ → False
⟨B⟩ → ( ⟨B⟩ )
⟨B⟩ → not ⟨B⟩
⟨B⟩ → ⟨B⟩ and ⟨B⟩
⟨B⟩ → ⟨B⟩ or ⟨B⟩
```

Denotational semantics (partially given):

```
Mₑ(⟨B⟩)  = 1       (for True)
Mₑ(⟨B⟩)  = 0       (for False)
Mₑ(⟨B⟩)  = ???     (complete the rest: parentheses, not, and, or)
```

> [!success]- Solution
> ![image-35.png|400x186](/img/user/1%20-%20MW%20CMP321/img/image-35.png)

---

**(b)** Apply your denotational semantics in part (a) to _evaluate_ the meaning/value of the expression `((A or B) and (not C))`, assuming A and C are `False` and B is `True`. Show _all_ the steps of your calculation. **(2 marks)**

> [!success]- Solution
> ![image-36.png|400x322](/img/user/1%20-%20MW%20CMP321/img/image-36.png)

---

### Exam 2: Question 5 — Python Expressions & Slicing

**(a)** Explain in detail the Python expression `x,y=[1,2j]`. You should describe all the steps clearly, in order, referring as needed to e.g., types, references, bindings, etc. Also, point out all the features that are unique to Python. **(7 marks)**

> [!success]- Solution
> Steps:
> 1. Right side is evaluated. A new list object is created storing the values [1,2j]. First element of array is integer 1. Second element of array is complex number: real part: 0 and imaginary part: 2.
> 2. Simultaneous assignment of x and y: x bind to first element of array, y bind to second element of array.
> In python, x and y are references that point to objects on heap. This simultaneous assignment of x,y is called "unpacking". You cannot perform this operation in C++/java. Also complex numbers are exclusive to Python. Also dynamic typing since x can be bound to any type of object without declaration and yet can still assign to type of array element (since it is all an object pointing to an object. In Python uniquely: all values are objects). Heterogeneous list: 2 different types (int and complex) in same list. The list syntax is unique as well.


---

**(b)** Write a Python expression that uses _slicing_ to produce `'13578642'` from the given string `s='12345678'`, or `'acdb'` if the string is `s='abcd'`, etc. (Assume that the input string always has an even length.) Point out what the equivalent code in C++ would be like, and hence the _benefits_ of slicing syntax. **(3 marks)**

> [!success]- Solution
> s\[0::2] + s\[-1::-2]
> 
> c++ equivalent:
> ```cpp
> for (int i=0; i<s.size(); i+=2) {
> 	cout << s[i];
> }
> for (int i=s.size()-1; i>=0; i-=2) {
> 	cout << s[i];
> }
> ```
> 
> benefit of slicing: removes the need for iterating through arrays using sequential statements (for/while loops). Therefore, saves time from writing longer lines of code and thus enhances writeability and readability since the intent is clear without tracing loop logic. Simpler appearance.

---

_End of Exam 2 (Midterm 1 A)_

---

## Exam 3: Midterm 2 (A)

---

### Exam 3: Question 1 — Python Expressions & Scripting

**(a)** Write a _single_ Python _expression_ for each task below. **(6 marks)**
- Retrieve the n _largest_ items from a tuple `t` of numbers
    
    ```
    e.g., n,t = 3,[2,6,11,3,17,0,8,13,5,10]  →  [11,13,17]
    ```
    
- Check whether a dictionary `d` has duplicate values or not (true or false)
    
- Given a list `ls`, print the tuples that consist of each list element and its position i.e., first element with number 1, etc. exactly as shown:
    
    ```
    e.g., ls=['a','b','c']  →  ('a', 1) ('b', 2) ('c', 3)
    ```

> [!success]- Solution
> ```python
> sorted(t, reverse=True)[n-1::-1]
> len(d.values())!=len(set(d.values())) #duplicates = true, no duplicates = false
> print(*zip(ls, range(1,len(ls)+1)))
> ```

---

**(b)** Write a Python script that rolls twenty dice and stores the frequency of each throw in a dictionary. Use `random.randrange()`, which has the same syntax as `range()`, to generate dice throws. Lastly, print the results formatted exactly as per the example shown below. Make sure your code is Pythonic. **(6 marks)**

```
1 : ****
2 : **
3 : ***
4 : ****
5 : *****
6 : **
```

> [!success]- Solution
> ```python
> dictionary={1:"", 2:"", 3:"", 4:"", 5:"", 6:""}
> for i in range(20):
>     roll = random.randrange(1,7)
>     dictionary[roll] += "*"
> 
> for k,v in dictionary.items():
>     print(f"{k} : {v}")
> ```

---

### Exam 3: Question 2 — Boolean Expressions & Zip

**(a)** Explain one feature of _Boolean expressions_ in Python which does not exist in C++ or Java. Illustrate the benefit with a well-chosen example. **(3 marks)**

> [!success]- Solution
> if not []:
>     print("empty")
> This works because an empty list is falsy.
> 
> Truthy/falsy values is a unique feature to python. The benefit in this case could be checking for empty strings, empty lists, etc. which would require a whole function in cpp/java. The Python form benefits: less verbose, works uniformly across all collection types (list, dict, str, set), no method call
> 
> Other valid answers: chained comparisons (1 < x < 10), or and/or returning operand values (e.g., 0 or 5 → 5, not True).

---

**(b)** Consider the Python code below. What are the lists `l1` and `l2` if the output is `[(1,2,3), ('a','b','c')]`? Explain briefly how this works. **(3 marks)**

```python
z=zip(l1,l2)
print(list(zip(*z)))
```

> [!success]- Solution
> ```python
> l1= [1,2,3]
> l2= ['a','b','c']
> z = zip(l1,l2) #list(zip(l1,l2)) = [(1,'a'), (2, 'b'), (3, 'c')]
> *z # = (1,'a'), (2, 'b'), (3, 'c')
> list(zip(*z)) # = [(1,2,3), ('a','b','c')]
> ```
> 
> l1 and l2 are zipped together.
> \*z unpacks the result of zip
> zip(\*z) zips the unpacked result of the first zip

---

### Exam 3: Question 3 — Functions: Multiple Returns, Overloading & `len`

**(a)** Contrary to C++ and Java, Python functions can return _multiple values_. Is that statement correct? Explain in detail using an example. **(3 marks)**

> [!success]- Solution
> statement is NOT technically correct. What looks like multiple returns is actually tuple packing on return + tuple unpacking on assignment.
> def f():
>     return 1, 2          # equivalent to: return (1, 2)
> 
> x = f()                  # x is the tuple (1, 2) — ONE object
> a, b = f()               # tuple unpacking on RHS — looks like 2 returns
> print(type(f()))         # <class 'tuple'>

---

**(b)** Write _two_ Python functions that mimic the C++ functions below as closely as possible. Explain what will happen exactly when the interpreter will evaluate your code. What does this example demonstrate clearly? **(4 marks)**

```cpp
int fun( int a ) { return 1 + a; }
int fun( int a, int b ) { return 1 + a*b; }
```


> [!success]- Solution
> def fun(a): return 1+a
> def fun(a,b): return 1+a\*b
> 
> The second def fun OVERWRITES the first. Function names in Python are just variable bindings, the second definition rebinds fun to the two-arg version. The one-arg version is now gone. This demonstrates: Python doesn't have method/function overloading. Unlike C++/Java, Python dispatches by name only, not by signature.


---

**(c)** Give then explain the output of the two Python expressions `len([1,3,5])` and `len(135)`. Explain accordingly what the `len` function really is. **(3 marks)**

> [!success]- Solution
> len([1,3,5]) will check number of elements in the list (OUTPUT: 3)
> len(135) will not work as there is a TypeError: object of type 'int' has no len().
> 
> len is a built-in function that delegates to the object's \_\_len\_\_ method (a dunder method). Lists, strings, tuples, dicts, sets all implement \_\_len\_\_, so len(x) works. Integers don't implement \_\_len_\_, hence the TypeError

---

### Exam 3: Question 4 — OOP: Class Design & Inheritance

**(a)** Implement a Python class called `T`, exactly as specified hereafter. Make sure to use standard OOP and Python coding and naming practices. **(8 marks)**

- Class `T` has a "private" _member variable_ to store the instance's name, which must be a user-provided string, or else a `TypeError` exception will be raised.
- Class `T` also has a "private" _class variable_ to store the names of all current and past instances of the class. Each name can be used only once. If one attempts to reuse a previous name, a `ValueError` exception will be raised.
- Class `T` implements a function to allow printing a class instance, exactly as shown below. The function should work just the same even if subclassing.
- Class `T` has a function that returns all current and past names, as shown below.

```python
t=T('one') ; print(t)    →  T instance with name "one"
print(T('two'))           →  T instance with name "two"
print(T.names())          →  ['one', 'two']
more = T('one')           →  ValueError: name already used
```

---

**(b)** Define `X`, a minimal subclass of `T` that adds a "public" `size` attribute. **(4 marks)**

---

### Exam 3: Question 5 — Functional Programming & Higher-Order Functions

**(a)** Explain _each step_ of the Python expression below, _in order_, stating what it does exactly and showing what data it produces. **(5 marks)**

```python
list(map(lambda t: str(Fraction(*t)), enumerate(range(1,9,2))))
```

> [!success]- Solution
> what it does:
> ```python
> #(1) get (index, range value) 
> enumerate(range(1,9,2)) # => (0, 1), (1, 3), (2, 5), (3, 7)
> #(2) tuple unpack each (index, range value) combination t and feed to Fraction function, then convert to string.
> lambda t: str(Fraction(*t)) # str(Fraction(*(0,1))) => str(0) => "0"
> # str(Fraction(*(1,3))) => str(1/3) => "1/3"
> 
> #(3) map each tuple to lambda function
> map(...)
> #(4) convert to list to force map(...) to apply for each. This is because map is a lazy iterator
> list(...)
> 
> #it produces a list value and this is what it looks like
> ["0","1/3","2/5","3/7"]
> ```

---

**(b)** For each task below, write a _single expression_ using Python functions and higher-order functions (but _not_ comprehensions) to yield the result. **(5 marks)**

- Give the number of family members older than a given age threshold `t`
    
    ```
    e.g., t=21, family = ({'name': 'Alice', 'age': 23},
                           {'name': 'Bob', 'age': 27},
                           {'name': 'Charlie', 'age': 18})  →  2
    ```

> [!success]- Solution
> ```python
> len(list(filter(lambda m: m['age']>t, family)))
> ```
> 
- Add all the bits of the binary representation of an integer N (using the `bin` function e.g.: `bin(5)` returns `'0b101'`, `bin(13)` returns `'0b1101'`, etc.)
    
    ```
    e.g., N=5 → 2,  N=13 → 3,  N=127 → 7
    ```
    
> [!success]- Solution
> 
> ```python
> reduce(lambda x,y: int(x)+int(y), bin(N)[2:])
> ```

---

_End of Exam 3 (Midterm 2 A)_

---

## Exam 4: Midterm 1 (B)

> **📌 Source:** M1_or_2.pdf — 6-page exam paper

---

### Exam 4: Question 1 — Python Expressions & Function Calls

**(a)** Indicate _what_ the expression below will produce, if `x` is a `float` object. List out every function call, in order, and state what each does exactly. **(4 marks)**

```python
len(str(x).split('.')[-1])
```

> [!success]- Solution
> ![image-38.png|400x338](/img/user/1%20-%20MW%20CMP321/img/image-38.png)

> [!success]- Alternative solution
> x=1.1
> y=1.12
> 
> len("1.1".split(.)[-1]) -- len(1) = 1
> len("1.12".split(.)[-1]) -- len(12) = 2
> 
> "1.12".split(.) = ["1","12"]   => [-1] takes the last element of list "12"
> 
> Therefore, this function will always take the number of digits after the decimal place.
> 
> inner is evaluated left to right. then outer len(...) is evaluated.
> 
> 1. str(x) converts the float to string so len(...) can work.
> 2. .split('.') splits string into array, first element the number before the . and the second element is the number after the .  
> 3. [-1] indexes the last element (fractional part)
> 4. len(...) takes length of the last element of list

---

**(b)** Indicate briefly but clearly _what_ each of the Python expressions hereafter represents, and what makes it _unique_ to Python (vs. C++ or Java). **(4 marks)**

- `[66, [], ]`
- `1+7j`
- `'say "hi"!'`
- `[1]*10`

> [!success]- Solution
> - `[66, [], ]`
> Here you have different element types inside one array, which cannot exist in C++ or Java (where you would have to define one element type for each element of the array). This is a feature of dynamic typing (no type declaration, objects carry their own type at runtime) and because they are all of type object. Also, there is a trailing comma after \[], which isn't allowed in C++ or Java.
> 
> - `1+7j`
> In Java and C++, you do not have a built-in option for complex numbers as a datatype, whereas it is a feature in Python and can store values as real and imaginary.
> 
> - `'say "hi"!'`
> In Python, there is no char, only string. In C++ and Java using ' ' is for characters. Because of this, you can use " " normally in strings when you enclose strings with '. 
> 
> - `[1]*10`
> In Python, you can perform repetition natively. Meaning \[1] will be repeated 10 times. In Java and C++, however, you would need to program a loop function. 

---

**(c)** What is the _output_ of `print(range(20,4,-4))` in Python? Why? **(2 marks)**

> [!success]- Solution
> range(20,4,-4) 
> This is because in Python, you print the object's representation, and in this case, they are lazy objects (like map(), filter(), zip(), enumerate()) which all need list() to produce an actual list). Imagine you did range(1_000_000_000), you would need to allocate memory for a billion integers immediately. This way you generate each value only when needed, using almost no memory. 
> 
> To get it in the list form, you would need to do print(list(range(20,4,-4))).

---

### Exam 4: Question 2 — Python Strings, Tuples & Dictionaries ⭐

**(a)** Write a _single_ Python _expression_ for each task below. **(6 marks)**

- Check if a string is a palindrome or not, regardless of case. Examples:
    
    ```
    'Feed the Animals' → False;   'Step on NO pets' → True
    ```

> [!success]- Solution
> Assuming string is x
> 
> `x.lower().split(' ')==x.lower().split(' ')[-1::-1]` ✗ Checks word by word. We need character by character:
> 
> `x.lower().replace(' ','')==x.lower().replace(' ','')[-1::-1]`

- Check whether a tuple `t` has duplicates or not (true or false)

> [!success]- Solution
> `len(t)!=len(set(t))`
> - True: has duplicates
> - False: no duplicates
> (tuple and a set are different types — they'll never be `==`. Compare their **lengths** instead)
> 

- Given a dictionary `d`, print the tuples that consist of each dictionary key and value, in that order, exactly as shown:
    
    ```
    e.g., d={'a':1, 'b':2, 'c':3} → ('a', 1) ('b', 2) ('c', 3)
    ```
    
> [!success]- Solution
> `print(*d.items())`
-Basic unpacking wont work because you need to specify the number of variables and dedicate it accordingly. So here it will only work for 3 variables:
a, b, c = d.items()
print(a, b, c)

---

**(b)** Write a Python function that will create a dictionary grouping a list of key-value pairs into a dictionary of lists, where the keys are sorted. Make sure your code is Pythonic. Justify the _O()_ complexity of your function. **(6 marks)**

```
Example: colors = [('Y',1), ('B',2), ('R',3), ('G',4),
                    ('G',5), ('B',6), ('G',2), ('R',1)]
         → {'B': [2,6], 'G': [2,4,5], 'R': [1,3], 'Y': [1]}
```

> [!success]- Solution
> ```python
> def colorgroup(lst):
>     dictionary = {}
>     for k, v in lst:
>         if k in dictionary:
>             dictionary[k].append(v)
>         else:
>             dictionary[k] = [v]
> 
>     result = dict(sorted(dictionary.items()))
>     for k in result:
>         result[k].sort()
>     return result
> ```
> 
> Complexity: O(n) loop + O(k log k) for sorting keys + O(n log n) total for sorting values across all lists → O(n log n) overall.



---

### Exam 4: Question 3 — Iterators & Generators

**(a)** Give the _output_ of the sample for loop below. Explain clearly how the code works i.e., give all the key steps, from the for loop itself to the methods of class `S` (as and when they are called). What does `S` do then? **(7 marks)**

```python
class S:
    def __init__(self, data, N):
        self.data, self.index, self.step = data, 0, N
    def __iter__(self): return self
    def __next__(self):
        if self.index >= len(self.data): raise StopIteration
        self.index += self.step
        return self.data[self.index - self.step]

for item in S(range(2,24), 5) : print(item, end=' ')
```

---

**(b)** Implement the `repeat` _generator_. Two typical use cases are shown below. Recall that the second argument to repeat, if provided, is the number of repetitions; without it, the generator is potentially infinite. **(5 marks)**

```python
list(repeat('@', 7)) → ['@', '@', '@', '@', '@', '@', '@']
set(map(pow, range(1,6), repeat(2))) → {1, 4, 9, 16, 25}
```

> [!success]- Solution
> def repeat(value, N=None):
>     if N is None:
>         while True:
>             yield value
>     else:
>         for _ in range(N):
>             yield value


---

### Exam 4: Question 4 — BNF Grammars & Derivations

**(a)** Describe precisely but concisely what the following BNF grammar rule generates, using simple, natural English (not programming jargon...) **(2 marks)**

```
⟨S⟩ → 0 ⟨S⟩ 1 | 01
```

> [!success]- Solution
> It is a BNF grammar rule that allows for strings of 0s and 1s that always start with 0 and end with 1. The rule will always make it so that the 0s come first and 1s come last. Also, the number of 0s will always equal the number of 1s
> Ex.
> 01
> 0011
> 000111

---

**(b)** Using the BNF grammar below, give a detailed left-most _derivation_ for the sentence `aaccdcc`. **(3 marks)**

```
⟨S⟩ → a ⟨S⟩ c ⟨B⟩
⟨S⟩ → ⟨A⟩ | b
⟨A⟩ → c ⟨A⟩ | c
⟨B⟩ → d | ⟨A⟩
```

> [!success]- Solution
> ![image-39.png|400x418](/img/user/1%20-%20MW%20CMP321/img/image-39.png)

---

**(c)** Show a _reverse derivation_ to prove that the sentence `acdc` cannot be produced by the grammar in part (b). Explain the error precisely. **(3 marks)**


> [!success]- Solution
> only rule 1 is where the grammar starts with a / allows for "a". So we have to make it in that form 
> ```
> a           c d c
> a           <A> d c
> a           <S> d c 
> ```
> ✗ error d cannot be before c. 
> This is because rule 1 expects a \<S> c \<B>. This is not possible
> 

---

_End of Exam 4 (Midterm 1 B)_

---

## Exam 5: Final Exam (B) — 11 Pages

> **📌 Source:** M1_or_2.pdf — 11-page exam paper

---

### Exam 5: Question 1 — Floor Division & Language Costs

**(a)** Explain clearly but concisely how the three expressions below compare in terms of _readability_, _writability_, and _reliability_. **(5 marks)**

```
x//y       vs.       Math.floor(x/y)       vs.       int(x/y)
```

> [!success]- Solution
> - readability: Math.floor(x/y) > int(x/y) > x//y.
> 	- Math.floor(x/y) explicitly states what operation will be placed on x and y. Readers can clearly read in a natural language style what the function is doing without any programming knowledge required.
> 	- int(x/y) lacks the description that Math.floor(x/y) has in stating what the function does directly, however, any reader can still make a conclusion on what the function does by knowing that whatever value x/y results in, will be converted to integer. 
> 	- x//y has the least readability as without any Python knowledge, // can be interpreted in different ways. Especially that // in other languages like C++ and Java is used for comments.
> - writability: x//y > int(x/y) > Math.floor(x/y).
> 	x//y is the most writable as it takes the least amount of time to write. It uses less lines of code to perform the same as the rest. It is more expressive by having a single convenient operator for it, as opposed to Math.floor(x/y) where you need to call the library then function name, or int(x/y) where you have to convert the function to int.
> - reliability: Math.floor(x/y) > x//y > int(x/y).
> 	x//y has a risk of typos due to its close similarity in spelling with x/y. Therefore, it is more prone to human errors. int(x/y) can introduce bugs since you are performing a function that was not intended for floor conversion. Also, for negative numbers, will result in an incorrect result silently (silent bugs), since it will truncate toward zero rather than perform floor divison. Math.floor(x/y) has the least error likelihood as it is the least confusing, it's less ambiguous than the rest and thus lowers rate of misunderstanding. Explicit is safer than implicit.
> 
> 	if x=-7, y=2:
> 	- x//y = Math.floor(x/y) = floor(-7/2)=-4
> 	- int(x/y)=truncate(-7/2) = -3

---

**(b)** Consider the five _cost criteria_ for programming languages that are: training, coding, tools, execution, and reliability. Explain briefly for each whether it has generally increased or decreased over the last decades, and why. **(5 marks)**

- **Training:**
- **Coding:**
- **Tools:**
- **Execution:**
- **Reliability:**

> repeated

---

### Exam 5: Question 2 — Raw Strings, Assignment & Slicing

**(a)** What is a _raw string_ in Python and what exactly is its purpose? Explain clearly using an appropriate example of your choosing. **(3 marks)**

> repeated

---

**(b)** Explain what the expression `x='y'` does in Python vs. the same in C++ (state your assumptions, if any). Point out what design decision/s this example illustrates, then give one advantage and one drawback for each. **(4 marks)**

> [!success]- Solution
> Python: x='y', makes it so that the variable x is now referencing the value of object y that the value of which is of type string.
> C++: x='y' makes it so that the value of variable x is equal to char 'y'
> 
> 
> Python's preference of string over char sacrifices performance for the sake of making it more convenient to the user. Although y is just one character, since it is stored as a string, it will have more memory usage. Since there is one type for text, it is simpler for rules to follow. It also follows a more orthogonal approach since 'y' and 'yy' are both strings. If they allowed for chars and strings, features like concatenation would be more unorthogonal since 'y'+'y' would turn chars into a string.
> 
> C++ tends to prefer performance over other factors like user convenience. The inclusion of char results in less memory usage and thus faster performance, but introduces orthogonality issues in concatenation functions and any similar operations with characters. Also more prone to user errors as '' is meant for chars, but "" is for strings and thus there are more rules to follow.
> 
> ~~(OPTIONAL):
> Python's method of making all variables references to objects allows for dynamic typing, where type checking is enforced at runtime. This method allows for smoother compilation of code, which can be useful if you're working on a certain part of the code and do not need to compile the whole code. However, This can introduce silent bugs as errors won't be noticed until the error case is met.~~
> 
> ~~C++'s method allows for static typing, where type checking is enforced at compile time. This prevents silent bugs as all cases are handled (error cases are found). However, this tends to take longer to compile.~~
> 


---

**(c)** Write a _single_ Python expression using _slicing_ for each case below. Note that your expression should work regardless of the string length. **(5 marks)**

- before: `s='ttAxxByyCzz'` → after: `s='ABCxyz'`

> [!success]- Solution
> `s=s[2::3]+s[3::3]`

- before: `l=[0, 2, 0, 4, 0, 6]` → after: `l=[1, 2, 3, 4, 5, 6]`

> [!success]- Solution
> [0,2,0,4,0,6,0] - odd
> `l[::2]=range(1,len(l)+1,2)`

---

### Exam 5: Question 3 — Recursive minmax & Fibonacci via reduce

**(a)** Write a _recursive_ `minmax` function in Python that returns _both_ the smallest and largest items from a given iterable. Make sure your code works in _all_ cases, and uses the language features (but not `min` or `max`, of course). **(6 marks)**

> [!success]- Solution
> ```python
> def minmax(itera):
> 	# if empty
> 	if not itera:
> 		return None, None
> 	# if len=1
> 	if len(itera)==1:
> 		return itera[0], itera[0]
> 	
> 	rest_min, rest_max = minmax(itera[1:])
> 	
> 	new_min, new_max = itera[0], itera[0]
> 	
> 	new_min = rest_min if rest_min < new_min else new_min
> 	new_max = rest_max if rest_max > new_max else new_max
> 	
> 	return new_min, new_max
> 	
> ```
	
---

**(b)** Indicate what `fun(N)` calculates, given the Python code below. Explain briefly the code logic, and especially what each step of reduce does exactly. Use the example of the call `fun(6)` to illustrate your answer in detail. **(6 marks)**

```
fun = lambda n: reduce(lambda x,n: (x[1], x[0]+x[1]),
                       range(n), (0,1)) [0]
```

> [!success]- Solution
> fun(N) calculates the Nth Fibonacci number. The reduce uses a tuple accumulator (F_k, F_{k+1}) because Fibonacci needs the previous two values. Each reduce step transforms (a, b) → (b, a+b), advancing the pair by one Fibonacci position. 
> 
> fun is storing a lambda function that takes a parameter N and then performs the following:
> 
> lambda x,n is the inner lambda performs computations to form a specific tuple
> - x=accumulator
> - n=current element from range(…) but it's never used.
> 
> range(n) is the iterable
> (0,1)         is the initializer
> 
> after reduce(…) the first element is taken from the tuple [0]
> 
> ```python
> fun(6)
> reduce(lambda x,n: (x[1], x[0]+x[1]),  #n is unused here
> 		range(6),   #iterable
> 		(0,1))      #initializer
> 		[0]         #extract index 0 of result
> 
> 	range(6) => 0,1,2,3,4,5
> 	
> 	(1,0+1) = (1,1) #element from range = 0
> 	(1,1+1) = (1,2) #element from range = 1
> 	(2,1+2) = (2,3) #element from range = 2
> 	(3,2+3) = (3,5) #element from range = 3
> 	(5,3+5) = (5,8) #element from range = 4
> 	(8,5+8) = (8,13) #element from range = 5
> 
> 	First element is taken : 8
> ```


---

### Exam 5: Question 4 — OOP: Docstrings & Comparable Interface

**(a)** Explain briefly but precisely what each line of the Python script below does, and give the output, or the error, if any. **(4 marks)**

```python
class alist: pass                    #1
lst = alist()                        #2
lst.__doc__ = 'the wiser'            #3
print(alist.__doc__, lst.__doc__)     #4
```

> [!success]- Solution
> #1 → Placeholder. Pass means 'do nothing'
> #2 → instance of `alist` stored in `lst`
> #3 → explain purpose of class (documentation)
> #4 → None. "the wiser"
> - None because there is no documentation
> - The wiser because that is what we set the documentation to.

---

**(b)** Explain the output of the print statement below, esp. what is compared and why. Define the `Comparable` abstract class that will act like a Java interface, then modify the `Point` class accordingly to "implement" this interface. Note that the same print statement should now show the correct result. **(6 marks)**

```python
class Point:
    def __init__(self, x=0, y=0): self.x, self.y = x, y
    def __str__(self): return f'[{self.x}, {self.y}]'

print(Point(1,2) == Point(1,2))
```

Write `Comparable` and modified `Point(Comparable)`:

```python
class Comparable(


class Point(Comparable):
    def __init__(self, x=0, y=0): self.x, self.y = x, y
    def __str__(self): return f'[{self.x}, {self.y}]'

    def
```

---

### Exam 5: Question 5 — Python Expressions & Slicing

**(a)** Explain in detail the Python expression `x,y=[1,2j]`. You should describe all the steps clearly, in order, referring as needed to e.g., types, references, bindings, etc. Also, point out all the features that are unique to Python. **(7 marks)**

---

**(b)** Write a Python expression that uses _slicing_ to produce `'13578642'` from the given string `s='12345678'`, or `'acdb'` if the string is `s='abcd'`, etc. (Assume that the input string always has an even length.) Point out what the equivalent code in C++ would be like, and hence the _benefits_ of slicing syntax. **(3 marks)**

---

### Exam 5: Question 6 — Reversed: Slicing vs Iterator vs Generator

**(a)** Point out what is _similar_ and what is _different_ between the two lines of code below given that e.g., `alist = range(1_000_000)`. **(3 marks)**

```python
for item in alist[::-1]: print(item)
for item in reversed(alist): print(item)
```

---

**(b)** Implement `reversed` as an _iterator_ so the above code works fine. **(5 marks)**

```python
class reversed:
```

---

**(c)** Now implement `reversed` as a simple _generator_ function. **(4 marks)**

```python
def reversed(data):
```

---

### Exam 5: Question 7 — Regular Expressions

**(a)** Describe, in simple English (not programming lingo), exactly _what kind of sentences_ match the regular expression: `"(0[xX])?[0-9a-fA-F]+"` **(2 marks)**

---

**(b)** Explain the two regular expressions `"\.(.*)\."` vs. `"\.(.*?)\."` and how they match an IP such as `"198.111.345.001"`. Show the results. **(4 marks)**

---

**(c)** Give the two _regular expressions_ `m` and `s` such that `re.sub(m,s,text)` will replace all _double_ occurrences of a word in the given text string by a _single_ occurrence of that word. Hint: use backward references. **(4 marks)**

```
Example:  'to be be or not to be, that is the the question'
        → 'to be or not to be, that is the question'
```

---

### Exam 5: Question 8 — BNF Grammar & Parse Trees

Given the following BNF grammar:

```
⟨sentence⟩   → ⟨subject⟩ ⟨predicate⟩
⟨subject⟩     → ⟨article⟩ ⟨noun⟩
⟨predicate⟩   → ⟨verb⟩ ⟨object⟩
⟨object⟩      → ⟨article⟩ ⟨noun⟩

⟨article⟩     → A | AN | THE
⟨noun⟩        → CAT | DOG | MAN
⟨verb⟩        → BITES | PETS
```

**(a)** Using the grammar above, draw a _parse tree_ to show that the sentence **THE MAN PETS A DOG** is in the language. **(3 marks)**

> redundant

---

**(b)** Prove that the sentence **DOG BITES MAN** is _not_ in the language. **(2 marks)**

> redundant

---

**(c)** The sentence **A MAN BITES THE DOG** _is_ also in the language, but we don't want that. How can we extend the grammar to exclude it? Explain briefly. **(3 marks)**

> redundant

---

**(d)** Is the above grammar _ambiguous_? Justify your answer. **(2 marks)**

> redundant

---

### Exam 5: Question 9 — Attribute Grammars (Fortran I Strings)

Character strings in Fortran I were expressed in the following format, where `⟨number⟩` is a positive integer, `H` is a literal key, and `⟨string⟩` is a sequence of one or more letters:

```
⟨string-literal⟩ → ⟨number⟩ H ⟨string⟩
```

Furthermore, a string literal is correctly defined _only_ if the value of `⟨number⟩` matches the length of `⟨string⟩`. For instance, `5Hhello` and `3Hbye` are valid character strings in Fortran I, whereas `2Hbad` and `10Hworse` are not.

**(a)** Indicate what kind of problems _attribute grammars_ are solving, then point out the specific issue in the case of Fortran I strings. **(3 marks)**

> [!success]- Solution
> Attribute grammars are solving semantic-related issues, including controlling the formatting and handling cases where syntax is correct, but logic is wrong. In this case, we can see for cases like 2Hbad and 10Hworse the syntax is correct `<number> -> H -> <string>` but the logic (number is length of string) is not represented.

---

**(b)** Give the necessary _attributes_, _predicates_, and _semantic rules_ (incl. look-up) of an attribute grammar for character string literals in Fortran I. **(6 marks)**

> [!success]- Solution
> Expand grammar first:
> ```
> ⟨string-literal⟩ → ⟨number⟩ H ⟨string⟩
> 
> <string> -> letter | <string> letter
> <number> -> digit  | <number> digit
> 
> ```
> 
> attributes:
> $.len \in \{1,2,3,\dots\}$
> $.val \in \{1,2,3,\dots\}$
> 
> semantic rules:
> 
> .len
> - base case: `<string> -> letter`
> 	- `<string>.len = 1`
> - recursive case: `<string> -> <string> letter`
> 	- `<string>[0].len = <string>[1].len + 1`
> 
> .val
> - base case: `<number> -> digit`
> 	- `<number>.val = lookup(digit)`
> - recursive case: `<number> -> <number> digit`
> 	- `<number>[0].val = <number>[1].val *10 + lookup(digit)`
> 
> predicates:
> `<string>.len==<number>.val`
> 
> > Note: lookup converts from a character, e.g. '4' (ASCII 52) to the integer 4 (numeric value).

---

**(c)** Draw the _decorated parse tree_ for the character string `4Hbad`, assuming that all attributes are synthesized. Show where the syntax error is found. **(3 marks)**

> [!success]- Solution
> ![image-42.png|400x351](/img/user/1%20-%20MW%20CMP321/img/image-42.png)

---

_End of Exam 5 (Final Exam B)_

---

## Exam 6: Midterm 2 (B)

> **📌 Source:** M1_or_2.pdf — partial exam paper (Q1–Q3 visible)

---

### Exam 6: Question 1 — OOP: Abstract Classes & Comparison Operators

**(a)** Write the code of the following three Python classes, exactly as specified. Make sure to use standard Python coding and naming practices. **(10 marks)**

- The abstract `Bird` class has a member variable to store a bird's name, which users must provide when creating a new bird. It has a class variable to store the sound every bird makes, which is `"chip"` by default. It implements a method to allow printing a bird's details, as per the examples below (and it cannot be overridden). The same method must be used by all concrete subclasses.
    
    ```python
    print(Dove('Love'))    →  Love the Dove says "cool"
    print(Duck('Huck'))    →  Huck the Duck says "kwak"
    ```
    
- The `Dove` class is a concrete subclass of `Bird` that has an additional `age` attribute, with a default value of `0`. It changes the sound every dove makes to `"cool"`.
    
- The `Duck` class is a concrete subclass of `Bird` that changes the sound every duck makes to `"kwak"`. It does not have any additional attribute.
    

---

**(b)** Explain how the class _comparison operator_ in Java vs. in Python are similar or different. Consider how/where they are defined, how they work... **(4 marks)**

---

### Exam 6: Question 2 — Functional Programming, Closures & Expressions

**(a)** Explain each step of the Python expression below (starting with the range) i.e., state briefly for each what it does and show what data it produces. Lastly, indicate how to modify the code minimally so as to add the terms together instead, producing a single number as result. **(5 marks)**

```python
list( map(lambda t: str(Fraction(*t)), enumerate(range(1,11,2), 1)))
```

> [!success]- Solution
> **RHS of map(…)**
> range(1,11,2) is a lazy sequence object that starts at 1 ends at 10 (11 exclusive) and skips every other element (step=2). 
> enumerate(range(…), 1) makes it so that it starts at 1. So the result in this case will look like this:
> (1, 1), (2,3), (3,5), (4,7), (5,9)
> 
> **LHS of map(…)**
> ```python
> lambda t: str(Faction(*t)) #equivalent to str(t[0]/t[1])
> ```
> 
> so when you map RHS with LHS, you will make each tuple go through the lambda funtion:
> ```python
> list(map(...)) # [str(1/1), str(2/3), str(3/5), str(4/7), str(5/9)
> #thus: ['1','2/3','3/5','4/7','5/9']
> ```
> 
> indicate how to modify the code minimally so as to add the terms together instead, producing a single number as result:
> ```python
> sum(map(lambda t: Fraction(*t), enumerate(range(1,11,2), 1)))
> ```
> 

---

**(b)** For each task below, write a single expression using Python functions, higher-order functions, and/or comprehensions, to yield the desired result. **(5 marks)**

- Calculate the average length of all iterables in a dictionary `d`
    
    ```
    e.g., d = {'A':[1,2,3], 'B':{4,5}, 'C':(6,7,8,9)}  →  3.0
    ```
    
- Calculate the sum of every other digits in a given integer `N`
    
    ```
    e.g., N = 1234567890  →  25    # because 1+3+5+7+9 = 25
          N = 73451       →  12    # because 7+4+1 = 12
    ```
    
> [!success]- Solution
> reduce(lambda counter,t: len(t)+counter, d.values(), 0)/len(d)
> 
> reduce(lambda a,b: int(a)+int(b), str(N)[::2])

---

**(c)** Explain what exactly is returned by the function below and what, accordingly, the print statement outputs, or which error is produced, if any. Explain how this relates to the use of global variables. **(4 marks)**

```python
def expB(base): return lambda exp: base**exp
e2=expB(2) ; del expB; print( e2(8) )
```

> [!success]- Solution
>del expB removes the name expB from the global namespace, but doesn't affect the lambda or its captured base=2 — e2 still holds a reference to the lambda, which still has the closure environment containing base. Hence e2(8) works, computing 2\*\*8 = 256."
> 
> Both closures and globals allow a function to access variables defined outside its own local scope.
> 
> Difference: closures capture from the enclosing function's scope (E in LEGB), not the global scope.
> 
> Here, we see it in the form of enclosing. Three conditions of enclosing are met: CONDITION 1: Nested function. CONDITION 2: inner function (in this case lambda function) must use variable from expB(base). CONDITION 3: outer function returns inner function.

---

### Exam 6: Question 3 — Higher-Order Functions: reduce & map

**(a)** Examine the function below and give the output of the two function calls. Explain briefly how this function works, justifying the use of `iter` and `try/except` in the code. Which well-known function does it implement? **(7 marks)**

```python
def mystery(function, iterable, initializer=None):
    it = iter(iterable)
    if initializer is None:
        try: value = next(it)
        except StopIteration: return
    else: value = initializer
    for element in it: value = function(value, element)
    return value

mystery(operator.add, [1,2,3,4,5])
mystery(operator.mul, [7,2,4], 10)
```

> [!success]- Solution
> reduce(…)
> 
> 1+2+3+4+5  OUTPUT OF LINE 1: 15
> [7,2,4] with initalizer as 10
> ```
> 10 * 7 = 70
> 70 * 2 = 140
> 140 * 4 = 560
> ```
> 
> OUTPUT OF LINE 2: 560
> 
> iter(iterable) converts the iterable into an iterator so you can call next() on it. 
> try/except: handle the case where the iterable is empty AND no initializer is given. In that case next(it) raises StopIteration. The except catches it and returns None (since reducing an empty sequence with no initial value has no defined result). Without this safety net, the function would crash on empty input.

---

**(b)** Implement `map` as a generator function, first **(i)** assuming that a single iterable is passed as argument, then **(ii)** in the general case, as shown below. **(5 marks)**

```
list(map(square, [1,2,3,4,5]))          → 1, then 4, 9, 16, and 25
list(map(pow, [2,3,5], [5,3,2]))        → 32.0, then 27.0, and 25.0
```

**(i)**

```
def map(function, iterable):
```

> [!success]- Solution
> ```python
> def map(function, iterable):
> 	for element in iterable:
> 		yield function(element)
> ```

**(ii)**

```
def map(
```

> [!success]- Full Solution
> i)
> ```python
> def map(function, iterable):
> 	for i in iterable:
> 		yield function(i)
> ```
> 
> ii)
> ```python
> def map(function, *iterables):
> 	for args in zip(*iterables):
> 		yield function(*args)
> ```

---

_End of Exam 6 (Midterm 2 B)_

---

## Exam 7: Midterm 2 (C)

> **📌 Source:** M1_or_2.pdf (6-page exam paper)

---

### Exam 7: Question 1 — Python Expressions & Uniqueness

**(a)** Indicate _what_ the expression below will produce, if `x` is a `float` object. List out every function call, in order, and state what each does exactly. **(4 marks)**

```python
len(str(x).split('.')[-1])
```

---

**(b)** Indicate briefly but clearly _what_ each of the Python expressions hereafter represents, and what makes it _unique_ to Python (vs. C++ or Java). **(4 marks)**

```python
[66, [], ]
```

```python
1+7j
```

```python
'say "hi"!'
```

```python
[1]*10
```

---

**(c)** What is the _output_ of `print(range(20,4,-4))` in Python? Why? **(2 marks)**

---

### Exam 7: Question 2 — Python Expressions & Dictionary Grouping

**(a)** Write a _single_ Python _expression_ for each task below. **(6 marks)**

- Check if a string is a _palindrome_ or not, regardless of case. Examples:
    
    ```
    'Feed the Animals'  →  False
    'Step on NO pets'   →  True
    ```
    
- Check whether a tuple `t` has _duplicates_ or not (true or false)
    
- Given a dictionary `d`, print the tuples that consist of each dictionary key and value, in that order, exactly as shown:
    
    ```
    e.g., d={'a':1, 'b':2, 'c':3}  →  ('a', 1) ('b', 2) ('c', 3)
    ```
    

---

**(b)** Write a Python function that will create a dictionary grouping a list of key-value pairs into a dictionary of lists, where the keys are sorted. Make sure your code is Pythonic. Justify the _O()_ complexity of your function. **(6 marks)**

```
Example:  colors = [('Y',1), ('B',2), ('R',3), ('G',4),
                    ('G',5), ('B',6), ('G',2), ('R',1)]
          → {'B': [2,6], 'G': [2,4,5], 'R': [1,3], 'Y': [1]}
```

---

### Exam 7: Question 3 — Comparisons (== vs is) & Pythonic Code

**(a)** Give the _value_ of each of the four conditional expressions hereafter. _Justify_ your answers briefly. **(3 marks)**

```python
n1,n2 = 10**6, 1_000_000

if n1 == n2 : ...
if n1 is n2 : ...

l1 = [1,2,3] ; l2 = l1[:]

if l1 == l2 : ...
if l1 is l2 : ...
```

> [!success]- Solution
> n1=10^6=10x10x10x10x10x10=1,000,000
> n2=1,000,000
> if n1 == n2 : TRUE. They have the same value (== is a value comparison operator)
> if n1 is n2 : FALSE. They are referencing different objects in memory (is compares memory location)
> 
> l1 = [1,2,3] ; l2 = l1[:]
> if l1 == l2 : TRUE. 
> if l1 is l2 : FALSE. l2 is a carbon copy of l1 (a new copy), and thus the location differs.


---

**(b)** ⭐ Give a more Pythonic version of the function below, and indicate _why_ it is _better_. Which programming paradigm is each version of the code (yours and the below) an example of? **(3 marks)**

```python
def max(a, b):
    if a > b:
        return a
    else:
        return b
```

> [!success]- Solution
> The above example is
> imperative/procedural
> 
> functional:
> def max(a,b):
> return a if a>b else b 
> 
> Ternary operator is better because it is more pythonic and is more writable and readable (since it requires less lines to read and write). Readability is also improved since it follows natural language more closely "return a if a is greater than b, otherwise return b"

---

### Exam 7: Question 4 — Function Parameters, F-Strings & Closures

**(a)** Explain one feature of _function parameters_ in Python which does not exist in C++ or Java. Illustrate the benefit with a well-chosen example. **(3 marks)**

> [!success]- Solution
> ![image-56.png|400x184](/img/user/1%20-%20MW%20CMP321/img/image-56.png)
> (1) more flexibility to the writer since he can write in any order he prefers
> (2) for when number of arguments is flexible. more user-friendly. \*\*kwargs collects extra keyword arguments for dictionary
> (3) clarity and safety

---

**(b)** Write a 1-line Python _function_ that takes a number as argument and returns an _F-string_ stating how many dogs one owns, exactly as shown below. **(3 marks)**

```python
print(own(1))      →  I have   1 dog
print(own(42))     →  I have  42 dogs
print(own(101))    →  I have 101 dogs
```

> [!success]- Solution
> ```python
> def own(num):
> 	return f"I have {num:>3} dog{'s' if num!=1 else ''}"
> ```

---

**(c)** Explain exactly _what is returned_ by the `greet` function below, what the print statements output, and _why_. Indicate, using this example, what the main _benefit_ of this design are, in terms of e.g., scope, reliability... **(4 marks)**

```python
def greet(msg='Hi'): return lambda to: msg + ', ' + to + '!'

print( greet()('Joe') )
g = greet('Hello') ; print( g('Sam') )
```

> [!success]- Solution
> greet function is performing a closure. It returns an inner lambda function that concatenates msg with ", " and to and "!". 
> 
> print(greet()('Joe')) prints "Hi, Joe!"          — because greet without parameters uses the default hi and ('Joe') is fed to the inner lambda function serving as `to`
> 
> print( g('Sam') )      prints "Hello, Sam!"    — because g is the result of closure.
> 
> The main benefit: 
> - scope: inner lambda function can use outer function variable (in this case msg) 
> - reliability: even if greet(…) function is deleted, g will remain functional and work as intended.
> 
> Closure conditions:
> 1. nested function
> 2. outer returns inner function
> 3. inner references outer function variable

---

### Exam 7: Question 5 — Higher-Order Patterns & Expressions

**(a)** Describe briefly the _three_ most common higher-order _patterns for repetition_ and name the functions that implement them in Python. **(4 marks)**

> [!success]- Solution
>      WHAT IT DOES        OUTPUT SIZE VS INPUT
> 1. Mapping → map()   — same length Transform each element by applying function
> 2. Filtering → filter       — same or shorter  Select elements that satisfy predicate
> 3. Reducing → reduce() — one value          Aggregate all elements into single value


---

**(b)** For each task below, write a _single expression_ using Python functions and higher-order functions (but _not_ comprehensions) to yield the result. **(8 marks)**

- Give the number of equal elements at the same index in two given lists
    
    ```
    e.g., n1,n2 = [1,2,3,4,5,6,7,8], [2,7,3,5,1,6,4,8]  →  3
    ```

> [!success]- Solution
> ```python
> len(list(filter(lambda x: x[0] == x[1], zip(n1, n2) )))
> ```

- Return the longest element in a sequence `s` of strings
    
> [!success]- Solution
>     ```
>     e.g., s=('papa', 'tango', 'charlie', 'over')  →  'charlie'
>     ```

```python
max(s, key=len)
```

- Count the number of elements in a list `l` that are larger than the average
    
    ```
    e.g., l = [4,1,2,10,5,8]  →  2
    ```

> [!success]- Solution
> ```python
> len(list(filter(lambda x: x>reduce(lambda a,b: a+b, l)/len(l), l) ))
> ```


---

_End of Exam 7 (Midterm 2 C)_

---

## Exam 8: Midterm 1 — Spring 2020 (Online)

> **📌 Source:** Midterm_1_-_Spring_2020.pdf (4 pages, 2-hour online exam)
> 
> **📌 Note:** Midterm_-_Spring_2020_Ramy.docx is a student's submitted answers to this same exam — questions are identical, so no separate entry is needed.

---

### Exam 8: Question 1 — Language Features, Popularity & Orthogonality

**(a)** Describe briefly one powerful feature which you discovered in Python and that does not exist in C++, but you wish it did. Explain which of the _"reasons for studying programming languages"_ this feature relates to and how exactly. Discuss the reason itself briefly i.e., what are the benefits, etc. **(4 marks)**

> [!success]- Solution
> Dynamic typing (which works alongside the fact that all variables are references to objects). It's nice to be able to switch between X="hi" to X=123 and have lists of varying element types like: \["user",123,1+2j]. It offers more flexibility for the developer, improving writability. It also doesn't lower readability (whereas C++ ways of circumventing the restriction through loopholes would instead lower readability like void*). The trade-off is reduced reliability from increased likelihood of human-caused silent bugs where you accidentally modify an existing variable. This relates to the "increased ability to express ideas" since developers can focus on problem itself rather than managing type declarations, allowing for natural expression.

---

**(b)** Several websites, such as Tiobe.com, track the popularity of programming languages and publish the results periodically. Explain how such information is useful for **(i)** programmers, **(ii)** language designers, and **(iii)** software project managers. Give some key benefits for each. **(5 marks)**

> [!success]- Solution
> **i) programmers**
> - They get to know the popular languages that jobs would likely seek. 
> - They get to know which are the leading languages depending on the type of programming language (database, general, etc.)
> - They get to discover new languages that they might've not known existed and learn them.
> 
> **ii) language designers**
> - Help understand user preferences, which can, in turn, help them know which features the language provides that users like.
> - Find most popular language of a category to develop a forked language (like typescript developers did with JavaScript) 
> - Understanding why certain languages got replaced over time and what people are focusing on (which can be an indicator of which languages will perform well as time goes on) 
> 
> **iii) software project managers**
> - Help establish which language a project should use for the categories (ex. picking the most popular one if the project necessitates third-party imports).
> - Help find a specific niche of a programming language that could be more suitable to the project (e.g. CoffeeScript)
> - Understand over time if the programming language will get replaced by another or does the language have a strong community and stayed #1 for a long time and thus will continue to be maintained (changing software code languages is an expensive task).

---

**(c)** Characterize and compare precisely the C program on the right with the Python script below in terms of _readability_, _writability_, and _reliability_. **(5 marks)**

```python
print(sum(range(1,66)))    # Python
```

```c
int sum=0, val=1;
while (val < 66)
  { sum += val;
    val += 1; }
print(sum);                // C
```

> [!success]- Solution
> **Readability**
> The Python code is more readable since it expresses the terms in a form that is syntactically similar to natural "Print the sum of the range from 1 to 66" (end value exclusive). The C version is less natural and the full function of each step isn't as easily described as the Python code: "Initialize the value of the variables sum to 0, val to 1, …"
> 
> Also, the Python code performs abstraction to reduce the code into one line, whereas the C code takes multiple lines (less abstraction), the former of which is easier for humans to read.
> 
> **Writability**
> The Python code requires less lines of code to implement the same function as C, and therefore it is more writable, reducing time for the developer to code. It also doesn't affect the flexibility, since you are still capable of mimicking the C code if the developer prefers using for loop and `range`.
> 
> **Reliability**
> Python code is more reliable than the C code.
> The C code has a higher likelihood of silent bugs since the more code you have to write, and the less readable it is, the higher chance of typos and other mistakes that are harder to detect (effect of readability/writability on reliability). C also has no built in bounds checking on the while loop, so you can create an infinite loop if you forget val+=1, while Python handles it for you so infinite loops aren't possible when you have to specify an end range.
> 
> **Cost**
> The C program has a higher barrier of entry to program it, therefore requiring more training costs (developer needs to understand while loops and the syntax, be aware of the int type as well as other types). 

---

**(d)** What does _orthogonality_ refer to in a programming language? Explain clearly using the examples of **(i)** _type conversion in Java_ and **(ii)** the usage of the _semicolon in C++_. **(6 marks)**

> [!success]- Solution
> Orthogonality: 
> 1. changing one component **doesn't** change another.
> 2. every possible combination is legal
> 
> **i) type conversion in Java**
> Unorthogonal.
> In Java, you can convert int to double, but not int to string. This means rules change depending on the type and context. An orthogonal design would allow ALL type conversions, or none. This situational rule is an un-orthogonal design.
> Also 1+"" is type conversion where changing one component changes another (it performs concatenation instead of mathematical addition).
> 
> **ii) usage of semicolon in C++**
> Unorthogonal.
> In C++, you have to use a semicolon after every line of code (statements, class definitions, do-while); however, there are exceptions: while loop, for, function definition, which do not require ";" after "{}".  Also in for loop semi colons are used to separate parts not end a statement.

> [!success]- Alternative Solution
> 1. orthogonality: consistency of rules 
>    a. every combination is legal (ex. if a rule applies to X type, it should apply to Y type as well). 
>    b. changing a component doesn't affect another
> 
> i) type conversion in Java does not follow the rules of orthogonality since some types can be converted but not others. For example: int x = 5.4 (int <- float conversion) works but string x = 5.4 (string <- float conversion) results in a TypeError.
> 
> ii) semicolon in C++ is unorthogonal because you write after every statement but in function declarations, sometimes in while loop, etc. you dont
> 
> do { } while(); <-- semicolon while() {} <-- no semicolon
> 
> int x = 5; <--- semicolon int func() {} <---- no semicolon

---

### Exam 8: Question 2 — Dynamic Typing, Type Inference & Python Expressions

**(a)** Explain exactly what _dynamic typing_ is, in Python, using the two lines of code shown on the right as example. **(3 marks)**

```python
x = 1
x = 'one'
```

> [!success]- Solution
> Dynamic typing, a native feature of Python (unlike C++ or Java), is where variable types are determined at runtime, allowing for the same variable to change types at runtime. This is allowed considering all variables in Python are references to objects. In the example we can see that x was initialized to the value of 1 of type int. Subsequently, it was rebound to a string with the value: "one".  It simply changed what it was referencing, and stopped pointing to the memory location of the object with the value 1.

---

**(b)** Explain what the C++ statement `auto x=1` does and contrast that with what the Python expression `x=1` does, _precisely_. Discuss accordingly similarities and differences of _type inference_ in C++ vs. Python. Your explanations should refer to e.g., types vs. values, static vs. dynamic… **(6 marks)**

> [!success]- Solution
> auto x=1 in C++ is type inference as opposed to x=1 in Python (dynamic typing). 
> Type inference just deduces based on the value, what the type of the variable would be, at compile time. It's more like predetermined rules (if x\==1, assign int). 
> Dynamic typing, on the other hand, means the type is determined at runtime. The type of the value is stored in the object itself, rather than the reference of the object (which is what is stored in variables).
> 
> Similarity:
> - they both achieve similar functions in terms of alleviating the programmer from the need to specify the type. 
> - both of them result in the same output. A result in integer type with value 1.
> 
> Difference:
> - `auto x=1` isn't dynamic  — it is still static. Whereas, Python's x=1 is indeed dynamic. This coincides with the general understanding that C++ is entirely static-typed language and Python is a dynamic-typed.
> - C++ type bound to variable (can never change). Python: type is bound to object (variable is reference that can point to anything).


---

**(c)** Indicate what each of the expressions hereafter represents and which are _unique to Python_ i.e., do not exist in C++ and Java. **(3 marks)**

```
(i)   "\u0078"
(ii)  [66,[],]
(iii) 1+7j
(iv)  N//2
```

> [!success]- Solution
> i → unicode escape sequence (not unique)
> ii → trailing comma, varying list types (unique)
> iii → complex numbers (unique)
> iv → floor function (unique)

---

**(d)** Explain in detail what the following Python statement does exactly and what its output is: **(3 marks)**

```python
'are scary movies worst at night?'[8:24:6]
```

> [!success]- Solution
> Slicing from the index 8 (9th char) to the index 23 (24th char) with steps of 6 (instead of the default 1). The output will be:
> yes


---

### Exam 8: Question 3 — List Replacement, Built-in Shadowing, Closures & Lambdas

**(a)** Consider the Python function below that replaces the elements from `alist` in the range `m..n` by the elements from the given `newlist` in the range `p..q`. Explain the _limitations_ of the function and show an example that will _not_ work. Rewrite it accordingly into a working, minimalist function. **(4 marks)**

```python
def sub(alist, m, n, newlist, p, q):
    for k in range(m,n):
        alist[k] = newlist[p-m+k]
```

> [!success]- Solution
> Example that it wont work:
> - m=0, n=3 ; p=0, q=1
> ```python
> for k in range(0,3):
> 	alist[k]=newlist[0-0+k]
> 	# alist[k]=newlist[0-0+0]  => [0]
> 	# alist[k]=newlist[0-0+1]  => [1] # ! OUT OF RANGE
> 	# alist[k]=newlist[0-0+2]  => [2] # ! OUT OF RANGE
> 
> # out of range is a problem because the index might not exist in newList and is not the expected behavior.
> ```
> 
> **Limitations**:
> - If the range of p..q is larger than the range of m,n then they wont replace all the elements with the full range of p..q newlist elements
> - If the range of p..q is smaller than the range of m,n then it will continue beyond the scope of newList range.
> This means for the ideal results, the range of p..q should be equal to the range of m..n
> - The original code never addresses the value of variable q.
> 
> **Minimalist function**
> alist[m:n]=newlist[p:q]
> 
> Python handles it: no loop, no out-of-range risk, no need for index math to introduce silent bugs. It automatically adjusts so that if newlist[p:q] is shorter than alist[m:n], the list on left hand side (alist) would grow or shrink accordingly 

> [!success]- Alternative Solution
> the value of q is not even considered here.
> 
> if range(m,n) = range(p,q) then this is the only situation where it works as intended.
> 
> if range(m,n) < range(p,q) then this will work but cause a silent bug since the newlist elements will not all be copied.
> 
> if range(m,n) > range(p,q) then this will not work since it will go outside the given range of newList and potentially out of bounds, causing an error.
> 
> An example of this would be if alist = [1,2,3] newList = [1,2] m=0, n=3 (since range is exclusive) p=0, q=2 then: alist[0]=newlist[0-0+0] alist[1]=newlist[0-0+1] alist[2]=newlist[0-0+2] #!ERROR (newList[2] out of bounds)
> 
> alist[m:n] = newlist[p:q]. This will shrink/expand the LHS list accordingly in case size mismatch.

---

**(b)** Explain why the following Python code snippets are _correct, or not_. **(3 marks)**

```python
zip = 26666 ; print('AUS P.O.', zip)
def printPO(name='AUS', zip=26666): print(name,'P.O. :', zip)
```

> [!success]- Solution
> The first Python code is correct and will work. The use of semi-colons in that sense is not considered Pythonic behavior though.
> This will always output AUS P.O. 26666 (comma automatically inserts a space)
> 
> The second Python code is also correct and will work. This has a different output and serves a different purpose (having AUS as the default name and zip as the default zip code, both of which can be overridden). Then if the function is called without parameters would print:
> AUS P.O. : 26666.
> 
> Both cases share a problem: shadowing. They replace Python's built-in zip() function for pairing up elements from two or more iterables. So although they work, it is not recommended to use built-in names like str, type, list, etc.

> [!success]- Alternative Solution
> it's correct as in they will print as expected. However, they both perform "shadowing" which means now Python's built-in zip(...) function cannot be called unless there was another variable referencing it. 
> OUTPUT OF LINE 1: AUS P.O. 26666
> Also, ; is unpythonic.


---

**(c)** Explain what each line below does, and state what is printed. **(3 marks)**

```python
def f(n): return lambda x: x**n     # line 1
print( f(3) )                       # line 2
print( f(3)(4) )                    # line 3
```

> [!success]- Solution
> ```
> #line 1 -> defines a function f that takes parameter n and returns an inner lambda function that takes x and calculates x**n
> 
> #line 2 -> this will print <function f.<locals>.<lambda> at 0x...> since this returns a "template" of the f function where n=3. This is because we didn't pass a value for the inner lambda function so a function is returned rather than a final result value.
> 
> #line 3 -> this will print the result 4**3=64. It simply calls the function with n=3 and passes 4 to lambda function so x=4.
> ```

---

**(d)** Give the main differences between Python _lambda expressions_ and _functions_. Accordingly, what is the intended use of lambda expressions in Python? Give two distinct usage examples. How is it different in Functional Programming languages, such as Haskell or Lisp? **(5 marks)**

> [!success]- Solution
> In Python, lambdas are deliberately restricted to a single expression — they're for short, throwaway anonymous functions. They're equivalent to a def that has just return expr.
> 
> lambda expression:
> 
> * cannot be named.
> * cannot be overly complex (multi-lines).
> * don't have a 'return ...' statement
> 
> functions:
> 
> * must have name
> * can be one line or multiple
> * can have a 'return ...' statement or not (void function)
> 
> They have different syntax as well.
> 
> lambda expression is used as quick function-like behavior but also provide unique characteristics like being used as a key for sorting.
> 
> sorted(lst, key=lambda entry: entry[0]) this will sort by the first character/digit of each element.
> 
> closure:
> def func(x):
>  return lambda y: y+x
> 
> Functional languages would have more focus on lambdas (given that lambda itself is a lambda FUNCTION). Therefore, they are a biger part of the core model of the language (ex. computation for haskell)
> 
> **🔁 REDUNDANT:** Similar to Exam 9 Q3(c).

---

### Exam 8: Question 4 — Square Class & Multiple Inheritance

**(a)** Write a minimal Python `Square` class so that the following code works as specified. All attributes should be "private" and the width should always be an integer value. The default width is _four_ but make sure we can change later if we wish to. Use standard Python coding and naming practices. **(7 marks)**

```python
s1 = Square()             # creates a new square of default width
s2 = Square(10)            # creates a new square with custom width (10)
print(len(s2))             # prints the square's current width
s3 = Square('ten')         # exception caught, error message printed
```

> [!success]- Solution
> ```python
> class Square:
>  default_width = 4
>  def __init__(self, width=None):
>   if width is None: width=Square.default_width
>   elif type(width) is not int: raise TypeError("ERROR: width should be integer.")
>   self._width=width
>   
>  def __len__(self): return self._width
>  
>  @classmethod
>  def change_def(cls, width): 
>   if type(width) is not int: raise TypeError("ERROR: width should be integer.")
>   cls.default_width = width 
> ```

> **🔁 REDUNDANT:** Variant of Exam 9 Q4(a) (default=1), Exam 10 Q4(a) (Count class).

---

**(b)** Write _two distinct_ Python expressions that will print the default square width: one that _is_ recommended and one that _is not_. Explain your code. **(3 marks)**

> **🔁 REDUNDANT:** Same as Exam 9 Q4(b).

---

**(c)** Describe briefly how Python allows for _multiple inheritance_ and how it differs from C++ and Java. Show which changes you should make to your `Square` class if it extends an abstract `Shape` class and a `Graphic` class. **(5 marks)**

---

### Exam 8: Question 5 — Expressions, Comprehensions & Higher-Order Concepts

**(a)** For each task below, write a _single statement_ using Python functions and features to yield the desired result. The simpler your code is the better. **(6 marks)**

- Prompt the user for words and return them in a string, as a comma-separated sequence, sorted alphabetically, all in lower case, without any duplicate
    
    ```
    e.g.: Hello bye tata cheers Bye  →  'bye,cheers,hello,tata'
    ```

> [!success]- Solution
> print(','.join(sorted(set(input().lower().split()))))

- Calculate the average length of all lists contained in a dictionary `d`
    
    ```
    e.g., d = {'A':[1,2], 'B':[3], 'C':[4,5,6]}  →  2
    ```
    
    > **🔁 REDUNDANT:** Same task as Exam 6 Q2(b).

> [!success]- Solution
> ```python
> sum(map(len, d.values()) )/len(d)
> ```

- Add all the numbers in a string
    
    ```
    e.g., s = "1.7 + 2 + 3.3 + 5"
    ```
    
> [!success]- Solution
> eval(s)

> [!success]- Alternative solution using HOF
> ```python
> reduce(lambda x, y: float(x)+float(y), s.split(' + ') )
> ```


---

**(b)** Use a Python _comprehension_ to realize each of the tasks below. **(4 marks)**

- Create an M×N matrix where the 1st row is a list of integers 1..N, the 2nd row is a list of their squares, the 3rd row is a list of their cubes, etc.
    
    ```
    e.g., for M,N=3,4  →  [[1,2,3,4], [1,4,9,16], [1,8,27,64]]
    ```

> [!success]- Solution
> `[[n**m for n in range(1,N+1)] for m in range(1,M+1)]`

- ⭐ Merge all dictionaries given in a list (assuming their keys are all different)
    
    ```
    e.g., dicts = [ {1:'a', 2:'b'}, {3:'c', 4:'d'}, {5:'e'} ]
          → {1: 'a', 2: 'b', 3: 'c', 4: 'd', 5: 'e'}
    ```

> [!success]- Solution
> `{ k:v for dictionary in dicts for k,v in dictionary.items() }`

---

**(c)** Explain how the concepts of _higher-order functions_, _comprehensions_, and _generators_ are related in Python. Use a code example to illustrate. **(5 marks)**

> [!success]- Solution
> HOFs express same idea as comprehensions but with different syntax.
> All generators are lazy. 
> 
> HOF: list(map(f, lst))
> Comprehension: [f(x) for x in lst]
> 
> HOF: list(filter(p, lst))
> Comprehension: [x for x in lst if p(x)]
> 
> The one HOF that doesn't have a comprehension equivalent is reduce because comprehensions produce collections, while reduce collapses to a single value
> 
> ---
> Generators are the lazy version of both HOFs and comprehensions
> map(f, lst) (without list())
> (x\*\*2 for x in range(n)) (generator expression -- tuples require comma this isnt tuple)

---

### Exam 8: Question 6 — Iterators, Flatten & Accumulate

**(a)** Explain the similarities and differences between _iterators_ in C++ and in Python, in terms of usage (e.g., for a range loop) and implementation. **(6 marks)**

---

**(b)** To _flatten_ a list means to remove one level of nesting. For example, `flatten([[1],[2,3],[4,5,6]])` should return the new list `[1,2,3,4,5,6]`.

**(i)** Code `flatten` using `reduce` and a lambda expression only. **(2 marks)**

```python
def flatten(
```

**(ii)** Now code `flatten` using a simple list comprehension. Indicate one small change to your code that would make `flatten` a _generator_ instead. **(3 marks)**

```python
def flatten(
```

**(iii)** Write a Python generator that takes any number of iterables as argument, returns elements from the first iterable until it is exhausted, then proceeds to the next iterable, etc. until all the iterables are exhausted. **(2 marks)**

```python
# chain('ABC','D','EF') should generate A B C D E F
def chain(
```

> **🔁 REDUNDANT:** Same as Exam 10 Q6(a) (`items()` variant).

**(iv)** Now code `flatten` using `chain` from part (iii) above. **(1 mark)**

```python
def flatten(
```

---

**(c)** Examine the Python function below and give the output of the following two expressions. Explain accordingly what the function does (summarize). Justify clearly the use of `iter`, `try/except`, and `yield` in the code. Which well-known function does it implement? **(6 marks)**

```python
def fun(iterable, op=operator.add):
    it = iter(iterable)
    try: result = next(it)
    except StopIteration: return
    yield result
    for element in it:
        result = op(result, element)
        yield result

for n in fun([2,9,5,4]): print(n, end=' ')
list(fun([2,9,5,4], operator.mul))
```

---

_End of Exam 8 (Midterm 1 — Spring 2020)_

---

## Exam 9: Midterm 1 — Spring 2021 (Online)

> **📌 Source:** Midterm_-_Spring_2021.docx (image-based, questions extracted from 13 embedded screenshots)

---

### Exam 9: Question 1 — Slicing, Reasons for Studying PLs, Case Sensitivity, Orthogonality & Compilation

**(a)** Describe briefly the _slicing_ feature available in Python, including which data structures it can apply to, and what it does exactly. Give two distinct examples i.e., RHS vs. LHS slicing, that demonstrate the power of this feature. **(4 marks)**

> [!success]- Solution
> Slicing mainly applies to ordered data structures including: lists, strings, and tuples (excluding dictionaries). 
> 
> Slicing extracts from the data structure a certain range of characters (for string) or elements (for lists and tuples). It can also perform jumps to skip a fixed number of characters ([1:10:5]  will skip 4 indexes every time it extracts an element)
> 
> RHS slicing: slice is on right side of the assignment
> X = sum(Y[1:3])
> 
> LHS slicing: slice is on left side of the assignment
> X[1:3] = [1,2,3]
> - It is worth noting that LHS slicing only works on lists (not strings or tuples since they're immutable). Rebinding (moving variable to new object) works, but not mutation (trying to modify the object itself).

note about regular slice vs extended slice

> [!success]- Solution
> ![image-44.png|400x332](/img/user/1%20-%20MW%20CMP321/img/image-44.png)

---

**(b)** Explain which of the _"reasons for studying programming languages"_ the slicing feature relates to and how exactly. Discuss the reason itself briefly, and what the benefits are, referring to your examples in part (a) again. **(4 marks)**

> [!success]- Solution
> Slicing relates to "increased ability to express ideas." This is because it gives the developer an easier access to extracting a substring (in a customizable way depending on the developer's needs), which can be useful in cases like taking the username from an email address, find last element in list easily, etc. This increased flexibility given to the developer with minimal code required, while maintaining human-friendly notation, facilitates the developer's capacity to express his ideas and perform the functions slicing was dedicated for. Features like slicing let us think at a higher level of abstraction rather than writing manual loops and thus relates to how studying different PLs expands how we think about solving problems.
> 
> As mentioned in a)
> X = sum(Y[1:3]) 
> adds the values of index 1 and index 2 of Y and assigns that value to X.
> Suppose Y was a list of earnings in one week, and we wanted to see how much was made on Tuesday and Wednesday and assign that value to a variable X. We would easily add the second and third element and add them.
> 
> X[1:3]
> Suppose X was an outdated list and some of the values needed to be corrected, we would reassign those values: in this case, replacing the values of 2nd element, 3rd element, and adds a new 4th element, containing 1,2,3 respectively.

---

~~**(c)** Modern programming languages distinguish _uppercase_ from _lowercase_ in identifiers such as variable and function names. What are the reasons for this design decision in terms of _readability_, _writability_, and _reliability_? **(6 marks)**~~

> **🔁 REDUNDANT:** Same as Exam 2 Q1 (case sensitivity).

---

**(d)** In C++, integer arguments are passed to a function by value whereas arrays are passed by reference. State how the same works in Python. Explain using this example what _orthogonality_ is, and why it matters. **(5 marks)**

> [!success]- Solution
> In Python, **everything is passed the same way (reference to object)** but the observable behavior differs based on mutability:
> - immutable: cant modify original (pass by value)
> - mutable: can modify original (pass by reference)
> 
> Orthogonality: 
> 1. changing one component doesn't change another. 
> 2. every possible combination is legal
> 
> C++ has an unorthogonal design because changing the type changes how it's passed (int vs array), whereas in Python it is orthogonal since it applies only one passing logic for all types of elements.


---

**(e)** List out the various _steps_ of the compilation process that starts with a Java source code file and ends with a running app. (Do not explain.) **(3 marks)**

> **🔁 REDUNDANT**: with Exam 2 Q2(b) 

---

### Exam 9: Question 2 — Dynamic Typing, Python Expressions, Slicing & Format

**(a)** Explain exactly what _dynamic typing_ is, in Python, using the two lines of code shown on the right as an example. Justify why it is possible, referring to the implementation of references. **(4 marks)**

```python
x = 'hi'
x = 1+j
```

> **🔁 REDUNDANT:** Same concept as Exam 8 Q2(a).

---

**(b)** Indicate _what_ each of the Python expressions below represents and which part is _unique_ to Python i.e., does _not_ exist in C++ and Java. **(3 marks)**

```
(i)   "don't"
(ii)  1+7j
(iii) ()
(iv)  N//2
```

> **🔁 REDUNDANT:** Overlaps with Exam 8 Q2(c), Exam 7 Q1(b).

only iii) is new:
> [!success]- Solution
> () as a literal syntax for creating an empty tuple is unique to Python. While C++ has tuples, Java doesn't, and C++'s tuple isn't easy to implement and not really natively built-in (requires you to include it).

---

**(c)** Explain _in detail_ what the following Python statement does exactly and what its output is: **(3 marks)**

```python
'are scary movies worst at night?'[8:24:6]
```

> **🔁 REDUNDANT:** Same slicing question as Exam 8 Q2(d), Exam 10 Q2(a), Exam 2 Q5.

---

**(d)** Give the arguments to the `format` function below and, accordingly, the _output_ of the following Python statement, or syntax error if any. **(3 marks)**

```Python
x,y = 17,5
print('{0}//{1}={2}, {0}%{1}={3}'.format(x,y,*divmod(x,y)))
```

> [!success]- Solution
> ```python
> x,y = 17,5
> print('{0}//{1}={2}, {0}%{1}={3}'.format(x,y,*divmod(x,y)))
> ```
> 
> .format is fed 4 values: x, y AS WELL AS quotient and remainder from divmod(x,y).
> 
> In this case, it's .format(17,5,3,2)
> Therefore,
> {0} = 17
> {1} = 5
> {2} = 3
> {3} = 2
> 
> Then it performs print(17//5=3, 17%5=2)
> 
> No syntax error, * is used to unpack

---

### Exam 9: Question 3 — mix() Function, Closures, Lambdas & Sorting

**(a)** Write a Python function `mix()` that takes a list of countries and a list of plates (1-letter abbreviations) as arguments and returns a dictionary matching their elements pair-wise as per the example below. **(4 marks)**

```python
countries, plates = ['spain', 'france', 'italy'], ['E', 'F', 'I']
mix(countries, plates)
#-> desired output: {'E': 'spain', 'F': 'france', 'I': 'italy'}
```

> [!success]- Solution
> ```Python
> def mix(countries, plates):
> 	return dict(zip(plates, countries))
> ```

---

**(b)** Explain what exactly is returned by the function below and what, accordingly, the print statement returns, or which error is produced, if any. **(3 marks)**

```python
def expB(base): return lambda exp: base**exp
e2=expB(2) ; del expB; print( e2(8) )
```

> **🔁 REDUNDANT:** Same closure question as Exam 6 Q2(c), Exam 10 Q3(c).

---

**(c)** Give the main _two differences_ between Python _lambda expressions_ and _functions_ and indicate, accordingly, what is their intended use. **(3 marks)**

> **🔁 REDUNDANT:** Similar lambda/function differences question in Exam 8 Q3(d).

---

**(d)** Using a lambda expression, write a single Python statement that will sort the numbers in `nlist` based on the _first decimal_, as illustrated below. **(5 marks)**

```python
nlist = [5.3, 1.48, 3.14, 2.2]
sorted(nlist)       # output: [1.48, 2.2, 3.14, 5.3]
# ???  -> desired output: [3.14, 2.2, 5.3, 1.48]
```

> [!success]- Solution
> `sorted(nlist, key=lambda x: str(x).split('.')[-1][0])`

---

### Exam 9: Question 4 — Square Class & Default Width

**(a)** Write a minimal Python class for square shapes so that the following code works as specified. The width attribute should always be an integer value. The default width is initially one but we should be able to change it as we wish using a class method. Make sure to write Pythonic code. **(7 marks)**

```python
s1 = Square()             # creates a new square of default width
s2 = Square(4)             # creates a new square with custom width 4
print(len(s2))             # prints the square's current width (e.g. 4)
s3 = Square('ten')         # exception caught, error message printed
```

> **🔁 REDUNDANT:** Variant of Exam 8 Q4(a), Exam 10 Q4(a) (Count class).

> [!success]- Solution
> ```python
> class Square:
>  default_width = 1
>  def __init__(self, width=None):
>   if (width==None): self.width=self.default_width
>   elif (type(width) is not int): raise TypeError("must be integer") 
>   else: self.width=width
>  
>  @classmethod
>  def change_val(cls, width):
>    Square.default_width = width
>  
>  def __len__(self):
>   return self.width
> ```


---

**(b)** Write two distinct Python expressions that will print the default square width: one that _is_ recommended and one that _is not_. Explain. **(3 marks)**

> [!success]- Solution
> ```python
> #1. Recommended
> print(Square.default_width) #simply accesses the default_width class variable of it.
> 
> #2. Not Recommended
> print(Square().default_width) #unnecessarily creates an object and makes it look like instance variable.
> ```

> **🔁 REDUNDANT:** Same default-width expression question in Exam 8 Q4(b).

---

_End of Exam 9 (Midterm 1 — Spring 2021)_

---

## Exam 10: Midterm 1 — Fall 2021

> **📌 Source:** Midterm_1_-_Fall_2021.pdf (5 pages, 50-minute exam, student-completed copy — handwritten answers ignored)

---

### Exam 10: Question 1 — Orthogonality (C++ vs Python)

In C++, integer arguments are passed to a function by value whereas arrays are passed by reference. State how the same works in Python. Explain using this example what _orthogonality_ is, and why it matters. **(5 marks)**

> **🔁 REDUNDANT:** Same question as Exam 9 Q1(d).

---

### Exam 10: Question 2 — String Slicing & Dictionary Comprehension

**(a)** Indicate what the following Python statement does and what its output is: **(2 marks)**

```python
'are scary movies worst at night?'[8:24:6]
```

> **🔁 REDUNDANT:** Same slicing question as Exam 8 Q2(d), Exam 9 Q2(c), Exam 2 Q5.

---

**(b)** Give the _output_ of the Python script below and state what the second line does, given that `dicts` is a list of dictionaries. What may be the issue? **(3 marks)**

```python
dicts = [ {1:'a', 2:'b', 5:'e'}, {3:'R', 7:'Z'} ]
print( {k: v for d in dicts for k, v in d.items()} )
```

> [!success]- Solution
> **OUTPUT:** `{1: 'a', 2: 'b', 5: 'e', 3: 'R', 7: 'Z'}`
> **Second line does:**
> It loops through each dictionary d in dicts, then loops through each key-value pair k, v in d.items(), and builds one merged dictionary using a dictionary comprehension. 
> 
> **May be issue:**
> If two dictionaries contain the same key, the later value overwrites the earlier one.

---

### Exam 10: Question 3 — Multiple Returns, Dictionary Dispatch & Closures

**(a)** Contrary to C++ and Java, Python functions can return _multiple values_. Is that statement correct? Explain in detail using an example. **(3 marks)**

> [!success]- Solution
> It's technically not true but functionally it seems to return multiple values BUT technically it does so through a single object: tuple.
> 
> def func():
>  return 10,20
> 
> x,y = func()
> 
> When a function returns x,y  , Python returns the values as a tuple so it's:
> x,y = (10,20)
> then performs unpacking:
> x=10, y=20  -> x and y are rebounded.
>
> RHS `1, 2` creates a tuple `(1, 2)` (tuple packing). The LHS `a, b` is a **target list** — Python's syntax for unpacking the RHS into individual names. So Python returns one tuple, and the LHS specifies how to unpack it

---

**(b)** Explain what the following Python script does exactly, step by step. **(4 marks)**

```python
options = { 1: cos, 2: sin, 3: tan }
print( options[ int( input("your choice? "))] (pi))
```

> [!success]- Solution
> This python lets the user decide which function (sin / cos / tan) to apply to pi based on the number it picks.
> 
> 1. options dictionary is defined with keys 1,2,3 and values cos, sin, tan respectively. 
> 2. user input is taken. If not 1,2,3 error will occur. If 1,2,3 proceed (input function results in string):
> 3. "1"/"2"/"3" converted to int:  1 or 2 or 3
> 4. options[1/2/3] and depending on that, either cos, sin, or tan function will be performed.
> 5. sin/cos/tan(pi) will be executed.
> 6. print(...) will output the result of step 5.


---

**(c)** Explain what exactly is returned by the function below and what, accordingly, the print statement returns, or which error is produced, if any. **(3 marks)**

```python
def expB(base): return lambda exp: base**exp
e2=expB(2) ; del expB; print( e2(8) )
```

> **🔁 REDUNDANT:** Same closure question as Exam 6 Q2(c), Exam 9 Q3(b).

---

### Exam 10: Question 4 — Count Class & Diamond Problem

**(a)** Write a minimal Python class to define counters, so that the following code works as specified. The count attribute should always be an integer value. The default starting value for counters is initially one, but we should be able to change it using a class method. Make sure to write Pythonic code. **(7 marks)**

```python
c1 = Count(10)               # creates a new counter starting at 10
c2 = Count()                  # creates a new counter with starting value of 1
c3 = Count('ten')             # exception raised → error message printed
Count.set_default(100)        # change default starting counter value to 100
c4 = Count()                  # creates a new counter, starting value is 100
print(c1)                     # prints the counter's current value e.g., 15
```

> **🔁 REDUNDANT:** Variant of the Square class in Exam 8 Q4(a), Exam 9 Q4(a).

---

**(b)** Explain briefly what the _diamond problem_ is in object-oriented programming, why it _must_ exist in Python, and _how_ the language solves the issue. **(3 marks)**

> **🔁 REDUNDANT:** Same question as Exam 1 Q7(a).

---

### Exam 10: Question 5 — Higher-Order Expressions & Patterns

**(a)** For each task below, write a _single statement_ using Python functions and features to yield the desired result. The simpler your code is the better. You should use _higher-order functions_ but _not_ comprehensions. **(6 marks)**

- Count the number of elements in a list `lst` that are larger than the average
    
    ```
    e.g., lst = [4,1,2,10,5,8]  →  2
    ```

> [!success]- Solution
> len(list(filter(lambda x: x>sum(lst)/len(lst), lst )))

    > **🔁 REDUNDANT:** Same task as Exam 7 Q5(b).
    
- Add all the comma-separated complex numbers contained in a string
    
    ```
    e.g., s = '1+2j, 3-5j, 5, 7+j'  →  (16-2j)
    ```
    
> [!success]- Solution
> reduce(lambda x,y: complex(x)+complex(y), s.split(', ') )

---

**(b)** Describe briefly the _three_ most common higher-order _patterns for repetition_ and name the functions that implement them in Python. **(4 marks)**

> **🔁 REDUNDANT:** Same question as Exam 7 Q5(a).

---

### Exam 10: Question 6 — Generators & StopIteration

**(a)** Write the Python _generator function_ `items()` that takes any number of iterables as argument, returns elements from the first iterable until it is exhausted, then proceeds to the next iterable, etc. until all the iterables are exhausted. **(4 marks)**

```python
# items('ABC', 'D', 'EF') should produce A B C D E F
def items(*args):
```

> [!success]- Solution
> ```python
> def items(*args):
>     for x in args:
>         for char in x:
>             yield char
> ```

> **🔁 REDUNDANT:** Same as Exam 8 Q6(b)(iii) (`chain()` variant).

---

**(b)** Write the _generator function_ `nested()` that takes a list of lists as argument and returns all the elements from the nested lists, in order. **(2 marks)**

```python
# nested([[1],[2,3],[4,5,6]]) should produce 1 2 3 4 5 6
def nested(lst):
```

> [!success]- Solution
> def nested(lst):
>     for x in lst:
>         for y in x:
>             yield y


---

**(c)** Write a _generator expression_ that is equivalent to `nested()` in part (b), without using `items()` or `nested()` itself, of course. **(2 marks)**

> [!success]- Solution
> `lstgen = (y for x in lst for y in x)`


---

**(d)** What is `StopIteration` in Python? **(2 marks)**

> [!success]- Solution
> StopIteration is an exception raised when an iterator or generator has no more values to produce. It is raised by next() when the iterator is exhausted. A for loop catches it automatically to stop iteration.

---

_End of Exam 10 (Midterm 1 — Fall 2021)_

---

## Exam 11: Midterm 1 — Spring 2022

> **Source:** Programming_Languages_Midterm_S22.pdf (5 scanned pages with handwritten answers, CamScanner) **Format:** 5 questions, 13 marks each, 50 minutes

---

### Exam 11: Question 1 — C vs Python & Orthogonality

**(a)** Characterize and compare in detail the C program on the right with the Python script below in terms of _readability_, _writability_, and _reliability_. **(5 marks)**

```python
print(sum(range(1,66)))   # Python
```

```c
int sum=0, val=1;
while (val < 66)
{ sum += val;
  val += 1; }
print(sum);   // C
```

> **🔁 REDUNDANT:** Same C vs Python comparison as Exam 8 Q1(c).

---

**(b)** What is _orthogonality_ in a programming language? Give a definition and illustrate your point using the example of an assignment such as `X=Y`, in the case of both Java and Python languages. **(5 marks)**

> [!success]- Solution
> Orthogonality:
> 1. A change in a component does not affect another.
> 2. Any combination is legal and consistent.
> 
> In Java, X=Y with different types only works in some case (double X = int Y works but string X = int Y doesn't). Meaning that if X is an string, but Y is a int, you cannot perform the assignment. This is unorthogonal because it violates definition 2 of orthogonality (inconsistent design).
> 
> Python, on the other hand, follows a more orthogonal design, where X=Y works with any type on LHS or RHS owing to **rebinding**. This is because Python's variables are references to objects, so assignment works uniformly.
> 
> string var = int var ✓ (Python) ✗ (Java)
> 
> An ideal orthogonal design ensures that a feature must be consistent and tolerate each possible case. 

---

### Exam 11: Question 2 — lsub Function, auto vs x=1 & pprint

**(a)** Consider the Python function below that replaces the elements from `alist` in the range `m..n` by the elements from the given `newlist` in the range `p..q`. Explain the limitation of this function and show an example that will not work. Rewrite it accordingly into a working, minimalist function. **(5 marks)**

```python
def lsub(alist, m, n, newlist, p, q):
    for k in range(m,n): alist[k] = newlist[p-m+k]
```

> **🔁 REDUNDANT:** Same `lsub` function as Exam 8 Q3(a).

---

**(b)** Explain precisely what is _similar_ and what is _different_ between the C++ statement `auto x=1;` and the Python expression `x=1`. Your explanations should refer to e.g., types, references, static vs. dynamic… **(4 marks)**

> **🔁 REDUNDANT:** Same as Exam 8 Q2(b).

---

**(c)** Write a Python function that will print power values using the data from a given dictionary, formatted as per the example below. **(4 marks)**

```python
data = { -9:2, 5:7, 3:6, -2:12 }
pprint(data)
```

```
  --9^2  =       81
  --2^12 =     4096
  3^6    =      729
  5^7    =    78125
```

> Negative keys are prefixed with `--`, output is right-aligned, sorted by key.

> [!success]- Solution
> 
> ```python
> def pprint(data):
> 	for num,power in sorted(data.items()):
> 		expr=f"{"-" if num<0 else ""}{num}^{power}"
> 		print(f"  {expr:<6} = {num**power:>8}")
> pprint(data)
> # `<` for left-align, `>` for right-align
> ```

---

### Exam 11: Question 3 — Multiple Returns, **call**, Sorting & Closures

**(a)** Contrary to C++ and Java, Python functions can return _multiple values_. Is that statement correct? Explain in detail using an example. **(3 marks)**

> **🔁 REDUNDANT:** Same question as Exam 10 Q3(a).

---

**(b)** Explain what the "magic" `__call__` attribute is, with an example. **(3 marks)**

> [!success]- Solution
> magic `__call__` attribute is simply the code that determines how a function call is made in Python. Each function has this attribute. For example:
> 
> def func():
>  return 1
> x = func() # = func.`__call__`  (will return 1)
> print(x) # output: 1
> 
> The part that makes this magic is you can apply it to any class as well and blur the lines between objects and functions by defining def __call()__ in the class
> 
> class Adder:
>     def `__init__`(self, n):
>         self.n = n
>     def `__call__`(self, x):
>         return self.n + x
> 
> add5 = Adder(5)
> print(add5(3))    # 8 — instance called like a function

---

**(c)** Write a Python expression that will sort a list of numeric strings based on the _first decimal place_. Sorting the list `['5.7', '1.842', '3.14', '202.02']` for example must yield `['202.02', '3.14', '5.7', '1.842']`. **(4 marks)**

> **🔁 REDUNDANT:** Same as Exam 9 Q3(c).

> [!success]- Solution
> ```python
> sorted(['5.7', '1.842', '3.14', '202.02'], key = lambda item: item.split('.')[-1][0])
> ```

---

**(d)** Explain what exactly is returned by the function below and what, accordingly, the print statement outputs, or which error is produced, if any. **(3 marks)**

```python
def multiplier(x): return lambda y: x*y
m3 = multiplier(3); del multiplier; print(m3(5))
```

> **🔁 REDUNDANT:** Similar closure/deletion question as Exam 9 Q3(d).

---

### Exam 11: Question 4 — Square Class, Default Width & Subclass

**(a)** Write a minimal Python class for `Square` shapes so that the code below works as specified and the following specs are met: The width attribute is _always_ an integer value; it is _hidden_ from users. The _default_ width is initially one but we _can change it anytime_. Make sure to write proper Pythonic code. **(7 marks)**

```python
s1 = Square()          # creates a new square of default width
s2 = Square(10)        # creates a new square with custom width (10)
print(len(s2))         # prints the square's current width
s3 = Square('ten')     # exception caught, error message printed
```



> **🔁 REDUNDANT:** Same Square class as Exam 8 Q4(a), Exam 9 Q4(a).

---

**(b)** Write two different Python expressions that will print the _current_ default value for the square width, one using functions and one without any. **(2 marks)**

> **🔁 REDUNDANT:** Same as Exam 8 Q4(b), Exam 9 Q4(b).

---

**(c)** Define a subclass of the `Square` class that adds a `name` attribute. Implement the initializer only, that will take a name and width as parameters. Make sure to follow proper OOP and Python programming style. **(3 marks)**

---

### Exam 11: Question 5 — Higher-Order Patterns, Expressions & reduce

**(a)** Describe briefly the _three_ most common higher-order _patterns for repetition_ and name the functions that implement them in Python. **(3 marks)**

> **🔁 REDUNDANT:** Same as Exam 7 Q5(a), Exam 10 Q5(a).

---

**(b)** For each task below, write a _single expression_ using Python functions and higher-order functions (but _not_ comprehensions) to yield the result. The simpler your code is the better. **(6 marks)**

– Calculate the average length of all lists contained in a dictionary `d` e.g., `d = {'A':[1,2], 'B':[3], 'C':[4,5,6]}` → `2`

– Return the longest element in a sequence `s` of strings e.g., `s=('papa', 'tango', 'charlie', 'over')` → `'charlie'`

> **🔁 REDUNDANT:** Average length same as Exam 6 Q2(b), Exam 8 Q5(a).

---

**(c)** Explain the output of the following Python code in detail (all steps). **(3 marks)**

```python
l1, l2 = [2,3], ['a','b','c']
reduce(operator.add, map(operator.mul, l1, l2))
```

> [!success]- Solution
> ```
> #1 assignment using tuple unpacking. position by position:
> l1 = [2,3]
> l2 = [ 'a','b','c' ]
> 
> #2 string repetition
> reduce(operator.add, ['aa', 'bbb']) #map stops at shortest iterable -> 'c' is dropped
> 
> #3 add 
> 'aa'+'bbb'
> => OUTPUT: 'aabbb'
> ```
> 

---

_End of Exam 11 (Midterm 1 — Spring 2022)_

---


## Midterm 1 — Filtered Tables (Exams 12–15)

### Exam 12: Final A — May 2020 — 5 of 7 questions relevant

|#|Question|Status|Notes|
|---|---|---|---|
|Q1|Readability, Writability, Reliability & Costs|✅|Ch1: `A && !B` vs `A and not B`, `count=1` vs `int count=1`; pointer costs|
|Q2|Parallel Assignment, Stack, Fib, FuncPool, Bug|⚠️|(a) `a,b=b,a` ✅ 🔁 Exam 1 Q5(a) · (b–e) stack/fib/funcpool/type bug ❌|
|Q3|Reversed Iteration: Slicing, Iterator, Generator|❌||
|Q4|BNF to Regex: Email Addresses|❌|Regex = Week 13|
|Q5|Ambiguous Grammars & Parse Trees|✅|Ch3: ambiguity, parse trees, proof, unambiguous rewrite, BNF/EBNF/Attr Grammar for adjectives|
|Q6|Static vs Dynamic Semantics & Denotational|✅|Ch3: static vs dynamic semantics; denotational semantics Boolean eval 🔁 Exam 2 Q4|
|Q7|Lexical Analysis & Recursive Descent Parsing|✅|W4: tokenization C++ vs Python, left recursion fix, derivation|

### Exam 13: Final B — Unknown Semester — 4.5 of 7 questions relevant

|#|Question|Status|Notes|
|---|---|---|---|
|Q1|Hexadecimal BNF Grammar|✅|Ch3: BNF construction, proving grammar incorrectness|
|Q2|BNF Derivation & Proof|✅|Ch3: leftmost derivation, prove not in language 🔁 Exam 2 Q3(c-d)|
|Q3|Static vs Dynamic Semantics & Ternary Numbers|✅|(a) static vs dynamic 🔁 Exam 12 Q6(a) · (b) ternary BNF + semantic rules ✅|
|Q4|Fortran I String Attribute Grammar|✅|🔁 Exam 5 Q9 — identical question|
|Q5|(Not captured)|—||
|Q6|C++ Tokenization, State Diagrams & Regex|⚠️|(a) tokenization ✅ W4 · (b–c) state diagrams/regex ❌|
|Q7|Regex Descriptions & HTML Tag Correction|❌|Regex = Week 13|

### Exam 14: Final C — Unknown Semester — All 5 visible questions relevant

|#|Question|Status|Notes|
|---|---|---|---|
|Q1|(Not captured)|—||
|Q2|C++ Assignments BNF & Switch EBNF|✅|Ch3: BNF for cascading assignments, EBNF for switch, syntax diagrams|
|Q3|Postfix Expressions & Ambiguity|✅|Ch3: BNF interpretation, derivation, parse tree, reverse derivation, ambiguity|
|Q4|English Grammar Ambiguity|✅|Ch3: two parse trees, ambiguity proof, unambiguous rewrite|
|Q5|BNF to EBNF to Regex & Format Specifiers|⚠️|(a) BNF interpretation + EBNF conversion ✅ · regex part ❌ · (b) regex ❌|
|Q6|Roman Numeral Attribute Grammar|✅|Ch3: semantic rules, evaluation, predicates, decorated parse tree|

### Exam 15: Appendix — Both questions relevant

|#|Question|Status|Notes|
|---|---|---|---|
|A1|Palindrome BNF & Attribute Grammar|✅|Ch3: BNF limitations, attribute grammar with predicates|
|A2|Lexical Analyzer vs Parser|✅|W4: tokenization, ambiguity between sign and operator|

---

## Exam 12: Final A — May 2020

> **📌 Source:** CMP321_Finals.md — Final A: May 2020 Final Exam **📌 Format:** 7 questions, typed question text

file:///G:/My%20Drive/Semester%207/CMP321/X.%20Previouses/PL/PL%20Previouses/Previouses/Programming%20Languages/Pastpapers/CMP%20321/CMP%20321/CMP%20321%20Previouses/Exams/Final%20Exam/CMP321-FinalExamPaper.pdf

---

### Exam 12: Question 1 — Readability, Writability, Reliability & Cost Criteria

**(a)** In each case below, compare the two given versions of a programming language feature in terms of _readability_, _writability_, and _reliability_. **(6 marks)**

– Logical operators e.g.: `(A && !B)` vs. `(A and not B)`

> [!success]- Solution
> **readability**: `A and not B` and similar statements without symbols as operators is more readable than `A && !B` because it is written in natural language. Therefore, someone with minimal programming background can understand it.
> **writability**: using symbols through logical operators such as `A && !B` is more concise and writable as the use of symbols in place of words reduces the time it takes to write each line of code, which can ultimately make a huge difference if the use of symbols is frequent.
> **reliability**: using symbols through logical operators such as `A && !B` is more ambiguous and thus is more prone to human errors. Also, since it's symbols rather than natural language, typos are more likely to occur like one & instead of two &'s (&&) 

– Declaration expression e.g.: `count = 1` vs. `int count = 1`

> [!success]- Solution
> **readability:** count = 1 is simpler and more abstract (less visual clutter). But int count = 1 is self-documenting — the reader knows the intended type immediately without tracing the code."
> **writability**: having not to worry about declaring the type and having abstraction saves developer time to write and handle both concepts. Instead, the computer handles it for him. This saves developer time of accounting for the concepts, managing it in later segments of code, etc.
> **Reliability**: omitted type, where the compiler automatically handles it, has more errors, since it introduces a lot of silent bugs, where the developer can accidentally assign a value of different type to a variable. This can also be an issue for user-inputted values for input(). The handling happens at runtime, thus, errors will be caught in runtime rather than compile time (type declared version). This means that these mistakes can be silent for a large part of the code and the error might be faced later on in the future of the code and thus it will be harder to track the source of the bug.


---

**(b)** Consider the four commonly used _cost criteria_ for programming languages that are: training, coding, execution, and maintenance. Explain for each how it is affected by the availability of _pointers_ in the language. **(4 marks)**

1. training cost: higher. To use pointers, one must understand the concept entirely: including how it works, what the value and dereferenced values are and how to determine them, how to handle or delete them / point them to null, etc. 
2. coding cost: higher. To use pointers, developer must take the time to write it and handle it when it is no longer being used. This can sometimes take a toll when writing code especially if the use of pointers is frequent.
3. execution cost: lower. Like giving the option for developers to handle garbage collection, having developers handle pointers makes it so that they manually take care of the pointer when done with (rather than having the garbage collector systematically scan throughout runtime to know if it's being unused). 
4. maintenance cost: higher. Developers must constantly check edge cases to ensure pointers do not go out of the range (with data structures like linked list), etc. Pointers are a major source of memory leaks (forgetting to delete), dangling pointers (using freed memory), etc. are all hard to debug and maintain and can thus make maintenance costly.

---

### Exam 12: Question 2 — Parallel Assignment

**(a)** Explain what the Python statement `a,b=b,a` does _exactly_. **(2 marks)**

> **🔁 REDUNDANT:** Same as Exam 1 Q5(a) — tuple unpacking swap.

---

### Exam 12: Question 5 — Ambiguous Grammars & Parse Trees

**(a)** Explain briefly but clearly, using an example of your choosing, why the grammar of a programming language _cannot_ be ambiguous. **(3 marks)**

> [!success]- Solution
> Because the compiler needs a systematic way to do things. If there is more then one interpretation then the compiler cannot decide between them.
> 
> ```
> expr -> <expr> + <expr> | <expr> / <expr> | num
> ```
> 2+8/2 = 5
> 2+8/2 = 6
> These have two different results and thus a compiler needs to choose between them.

---

**(b)** Draw two distinct _parse trees_ to show that the sentence `'small cats and dogs'` is _ambiguous_ given the language grammar below. **(4 marks)**

```
⟨s⟩   → ⟨np⟩                  ⟨n⟩ → cats | dogs | birds |
⟨np⟩  → ⟨a⟩ ⟨np⟩                     hamsters | turtles
⟨np⟩  → ⟨np⟩ and ⟨np⟩         ⟨a⟩ → large | small | red |
⟨np⟩  → ⟨n⟩                          blue | brown | cute
```

> [!success]- Solution
> ![image-43.png|400x213](/img/user/1%20-%20MW%20CMP321/img/image-43.png)

---

**(c)** Prove that the sentence `'every cat and dog can play'` is _not_ in the language defined by the grammar in part (b) above. **(3 marks)**

> [!success]- Solution
> The words 'every', 'cat', 'dog', 'can', and 'play' are not terminals in any production rule, so no derivation from ⟨s⟩ can produce this sentence
> ```
> <s>
> <np>
> cannot proceed from here
> ```


---

**(d)** Rewrite the three `⟨np⟩` rules to make the grammar _unambiguous_. **(3 marks)**

> [!success]- Solution
> ```
> ⟨s⟩   → ⟨np⟩
> <np> -> <n>
> <np> -> <a> <np>
> <np> -> <n> and <np>
> ```

---

**(e)** The above grammar can generate sentences with _more than three adjectives_, such as `'cute small red blue birds'`, which we need to _disallow_. Explain how it can be done (i) in BNF, then (ii) in EBNF, and finally (iii) using an Attribute Grammar. Write all necessary rules and details. **(7 marks)**

> [!success]- Solution
> i) 
> add epsilon ε to \<a>
> ```
> ⟨s⟩   → ⟨np⟩
> <np> -> <a> <a> <a> <n>
> ⟨np⟩  → ⟨np⟩ and ⟨np⟩
> 
> <a> -> large | small | red | blue | brown | cute | ε
> <n> -> cats | dogs | birds | hamsters | turtles
> ```
> 
> ii)
> add optional 
> ```
> ⟨s⟩   → ⟨np⟩
> ⟨np⟩ → [⟨a⟩] [⟨a⟩] [⟨a⟩] ⟨n⟩ {and [⟨a⟩] [⟨a⟩] [⟨a⟩] ⟨n⟩}
> 
> <a> -> large | small | red | blue | brown | cute
> <n> -> cats | dogs | birds | hamsters | turtles
> ```
> 
> iii)
> 
> ```
> attributes:
> <np>.count ε {0,1,2,3}
> 
> semantic rules
> <np> -> <n>: <np>.count = 0                                  base case
> <np> -> <a> <np>: <np>[0].count = <np>[1].count + 1          recursive case
> ⟨np⟩ → ⟨n⟩ and ⟨np⟩: ⟨np⟩[0].count = 0
> 
> predicates
> <np>.count <= 3
> ```


---

### Exam 12: Question 6 — Static vs Dynamic Semantics & Denotational Semantics

**(a)** Explain precisely the difference between _static semantics_ and _dynamic semantics_ using the example of a C++ assignment e.g., `x=y`. **(3 marks)**

> [!success]- Solution
> Static semantics is the verification checks that happen during the compile time of the code. For example, these include: are the variables x and y declared and initialized? Are their types compatible? is X valid target?
> 
> Dynamic types is the execution behavior that happen during the runtime of the code. For example, these include: evaluate y value, find memory address of X, store value of y into memory location of X.

---

**(b)** Complete the rules of _denotational semantics_ below (right) to define Boolean operators. Apply the rules to _evaluate_ `((A or B) and (not C))`, assuming A and C are `False` and B is `True`. Show _all_ the steps of the evaluation. **(7 marks)**

```
⟨B⟩  →  True          Mₑ(⟨B⟩) = 1
⟨B⟩  →  False         Mₑ(⟨B⟩) = 0
⟨B⟩  →  ( ⟨B⟩ )      Mₑ(⟨B⟩)
⟨B⟩  →  not ⟨B⟩       Mₑ(⟨B⟩)
⟨B⟩  →  ⟨B⟩ and ⟨B⟩   Mₑ(⟨B⟩)
⟨B⟩  →  ⟨B⟩ or ⟨B⟩    Mₑ(⟨B⟩)
```

> redundant

---

### Exam 12: Question 7 — Lexical Analysis & Recursive Descent Parsing

**(a)** Show how a _lexical analyzer_ will tokenize the expression `F()//N++` if parsing C++ code _vs._ parsing Python code. Give all the tokens. **(4 marks)**

> [!success]- Solution
> C++
> 
> | F          | IDENTIFIER  |
> | ---------- | ----------- |
> | (          | LEFT_PAREN  |
> | )          | RIGHT_PAREN |
> 
> //N++ is a comment, gone. Parser never sees it.
> 
> 
> PYTHON
> 
> | F   | IDENTIFIER  |
> | --- | ----------- |
> | (   | LEFT_PAREN  |
> | )   | RIGHT_PAREN |
> | //  | OPERATOR    |
> | N   | IDENTIFIER  |
> | +   | OPERATOR    |
> | +   | OPERATOR    |
> 


---

**(b)** Explain what _issue_ will be encountered with the following BNF grammar rule when using a _recursive top-down parser_, then fix the problem. **(3 marks)**

```
⟨expr⟩ → ⟨expr⟩ + ⟨term⟩ | ⟨term⟩
```


> [!success]- Solution
> Immediate Left Recursion. infinite loop as it will always call \<expr>. 
> ```
> <expr> -> <expr2> + <term> | <term>
> <expr2> -> <term> + <expr> | <term>
> ```
> 
> OR officially:
> `⟨expr⟩ → ⟨term⟩ ⟨tail⟩`
> `⟨tail⟩ → + ⟨term⟩ ⟨tail⟩ | ε`

---

**(c)** Write the left-most derivation equivalent to that shown on the left, using the new rule/s in part (b). Assume we have a rule `⟨term⟩ → T | …` **(3 marks)**

```
⟨expr⟩ → ⟨expr⟩ + ⟨term⟩        
⟨expr⟩ → ⟨expr⟩ + ⟨term⟩
      → ⟨term⟩ + ⟨term⟩
      → T      + ⟨term⟩
      → T      + T
```

> [!success]- Solution
> part b rules + new rule
> > `⟨expr⟩ → ⟨term⟩ ⟨tail⟩`
> > `⟨tail⟩ → + ⟨term⟩ ⟨tail⟩ | ε`
> `⟨term⟩ → T | …` 
> 
> ```
> <expr> -> <term> <tail>
> 	      T      <tail>
> 	      T      + <term> <tail>
> 	      T      + T      <tail>
> 	      T      + T      ε
> 	      T      + T
> ```

---

_End of Exam 12 (Final A — May 2020)_

---

## Exam 13: Final B — Unknown Semester (Grammar-Heavy)

> **📌 Source:** CMP321_Finals.md — Final B **📌 Format:** Questions 1–7 (Q5 not captured)

---

### Exam 13: Question 1 — Hexadecimal BNF Grammar

**(a)** Complete the BNF grammar of _hexadecimal numbers_ below. **(2 marks)**

```
⟨digit⟩   → 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9
⟨letter⟩  → A | B | C | D | E | F

⟨hex⟩     → ?
```

> [!success]- Solution
> `<hex> - > ⟨digit⟩ | ⟨letter⟩ | ⟨hex⟩ ⟨digit⟩ | ⟨hex⟩ ⟨letter⟩`
> OR
> `<hex> -> <digit> | <letter> | <letter> <hex> | <digit> <hex>`

---

**(b)** Show exactly _why_ the grammar rule below is incorrect. **(4 marks)**

```
⟨hex⟩ → ⟨digit⟩ | ⟨letter⟩ | ⟨hex⟩ ⟨hex⟩
```

> [!success]- Solution
> Double recursion = ambiguous
> 
> ```
> 4FF
> 
> <hex> -> <hex> <hex>
>       -> 4     <hex>
>       -> 4     <hex> <hex>
>       -> 4     F     F
>       
> <hex> -> <hex>       <hex>
>       -> <hex>       <hex>
>       -> <hex> <hex> <hex>
>       -> 4     F     <hex>
>       -> 4     F     F
> 
> ```
> 
> Therefore there will be two distinct parse trees.


---

### Exam 13: Question 2 — BNF Derivation & Proof

**(a)** Using the BNF grammar below, write a detailed _left-most derivation_ to show that the sentence `'the cat likes to eat and play'` is valid. **(3 marks)**

```
⟨s⟩   → ⟨np⟩ ⟨vp⟩              ⟨d⟩  → a | the | every
⟨np⟩  → ⟨d⟩ ⟨n⟩                ⟨n⟩  → cat | dog | hamster
⟨vp⟩  → ⟨av⟩ ⟨v⟩               ⟨av⟩ → can | 'likes to'
⟨vp⟩  → ⟨av⟩ ⟨v⟩ and ⟨v⟩       ⟨v⟩  → eat | play | run
```

> **🔁 REDUNDANT:** Same grammar as Exam 2 Q3(c).

---

**(b)** Prove that the sentence `'every cat and dog can play'` is _not_ in the language defined by the grammar in part (a) above. **(3 marks)**

> [!success]- Solution
> ```
> <s> -> <np>     <vp>
>        <d>   <n>  <vp>
>        every <n>  <vp>
>        every cat  <vp>
>        every cat  <av>     <v> and <v> 
>        
>        X cannot proceed since <av> cannot be "and" nor can it be empty. The and is in a different grammatical position.
>        X the other <vp> fails since <av> also cannot be and
> ```


---

### Exam 13: Question 3 — Static vs Dynamic Semantics & Ternary Numbers

**(a)** Explain the difference between _static semantics_ and _dynamic semantics_ using the example of a C++ assignment e.g., `x=y`. **(3 marks)**

> **🔁 REDUNDANT:** Same as Exam 12 Q6(a).

---

**(b)** Ternary numbers have three possible values: 0, 1, and 2. For instance, 12 and 210 in ternary are 5 and 21 in decimal, respectively. Give a BNF grammar for ternary numbers and the corresponding semantic rules. Calculate accordingly the decimal value of the ternary number `1021`. Show all the steps. **(5 marks)**

> [!success]- Solution
> ```
> <S> -> <ternary>
> <ternary> -> <ternary> <digit> | <digit>
> <digit> -> 0 | 1 | 2
> 
> ---
> Attributes:
> ⟨ternary⟩.val ε {0,1,2,...}
> 
> Semantic rules:
> ⟨ternary⟩ → ⟨digit⟩: ⟨ternary⟩.val = ⟨digit⟩.val
> ⟨ternary⟩ → ⟨ternary⟩ ⟨digit⟩: ⟨ternary⟩[0].val = ⟨ternary⟩[1].val × 3 + ⟨digit⟩.val
> 
> ---
> ⟨ternary⟩ → ⟨ternary⟩ ⟨digit⟩(1)
>            → ⟨ternary⟩ ⟨digit⟩(2) ⟨digit⟩(1)
>            → ⟨ternary⟩ ⟨digit⟩(0) ⟨digit⟩(2) ⟨digit⟩(1)
>            → ⟨digit⟩(1) ⟨digit⟩(0) ⟨digit⟩(2) ⟨digit⟩(1)
>            
> Now let's do bottom-up approach since this is synthesized (inherited is top down)
> 
> 1. <ternary> -> <digit>: val = 1
> 2. <ternary> -> ⟨ternary⟩ <digit>: val = 1 x 3 + 0 = 3
> 3. <ternary> -> ⟨ternary⟩ <digit>: val = 3 x 3 + 2 = 11
> 4. <ternary> -> ⟨ternary⟩ <digit>: val = 11 x 3 + 1 = 34
> 
> ```

---

### Exam 13: Question 4 — Fortran I String Attribute Grammar

**(a)** Give the necessary _attribute(s)_, _predicate(s)_, and _semantic rule(s)_ (including look-up rules) of an attribute grammar for character string literals in Fortran I. **(4 marks)**

> Character strings in Fortran I were expressed in the following format, where `⟨number⟩` is an integer (≥1), H is a literal key, and `⟨string⟩` is a sequence of one or more letters: `⟨string-literal⟩ → ⟨number⟩ H ⟨string⟩` A string literal is correctly defined _only_ if the value of `⟨number⟩` matches the length of `⟨string⟩`.

> **🔁 REDUNDANT:** Same as Exam 5 Q9.

---

**(b)** Draw the _decorated parse tree_ for the character string `4Hbad` if all attributes are synthetized bottom up. **(3 marks)**

> **🔁 REDUNDANT:** Same as Exam 5 Q9(c).

---

### Exam 13: Question 6 — C++ Tokenization

**(a)** Draw a vertical bar after each lexeme to _tokenize_ the C++ expression below, and _label_ each element identified with the corresponding token. **(2 marks)**

```
void fun(int* x){ return --x>0; } // C++
```


> [!success]- Solution
> 
> | void    | fun        | (          | int     | *        | x          | )           |
> | ------- | ---------- | ---------- | ------- | -------- | ---------- | ----------- |
> | KEYWORD | IDENTIFIER | LEFT_PAREN | KEYWORD | OPERATOR | IDENTIFIER | RIGHT_PAREN |
> 
> 
> | {          | return  | --       | x          | >        |
> | ---------- | ------- | -------- | ---------- | -------- |
> | LEFT_BRACE | KEYWORD | OPERATOR | IDENTIFIER | OPERATOR |
> 
> | 0               | ;         | }           |
> | --------------- | --------- | ----------- |
> | INTEGER_LITERAL | SEMICOLON | RIGHT_BRACE |
> 
> // C++ → COMMENT (discarded by lexer)



> **Note:** Parts (b) state diagrams and (c) regex are ❌ not M1 scope.

---

_End of Exam 13 (Final B)_

---

## Exam 14: Final C — Unknown Semester (BNF & Attribute Grammars)

> **📌 Source:** CMP321_Finals.md — Final C **📌 Format:** Questions 2–6 captured. Q1 not in images.

Turned out to be homework 2 not final...

---

### Exam 14: Question 2 — C++ Assignments BNF & Switch EBNF

**(a)** Write BNF rules to define simple _assignments_ in C++, which may _cascade_. Valid examples include: `a=0; b=c; m=n=12; x=y=z;` (with the semi-colon). Assume the non-terminals `⟨const⟩` for numeric constants and `⟨var⟩` for variables are given. Is your grammar left-recursive? Explain. **(2 marks)**

> [!success]- Solution
> ```bnf
> <sentence> -> <var> = <xpr>
> <xpr> -> <var>; | <sentence> | <const>;
> ```
> My grammar is right recursive because the recursive non-terminal is at the end of the syntax.
> 
> ```
> m=n=12
> <var> = <xpr>
> m = <xpr>
> m = <sentence>
> m = <var> = <xpr>
> m = n = <xpr>
> m = n = <const>;
> m = n = 12;
> ```
> No ambiguity. Only one parse tree.
> 
---

**(b)** Write EBNF rules for a _switch_ statement in C. Note that it is _not_ the same as C++; look up the definition if you need. Assume the following non-terminals are given: `⟨expr⟩` representing any valid C expression and `⟨stmt-list⟩` for a list of C statements. Draw the equivalent _syntax diagrams_. **(3 marks)**

> [!success]- Solution
> ```e bnf
> <statement> -> 'switch (' <expr> ') {' {'case' <const>':' <stmt-list>} ['default:' <stmt-list>] '}'
> ```

---

### Exam 14: Question 3 — Postfix Expressions & Ambiguity

**(a)** Indicate _what_ the context-free grammar below (BNF) _generates_, and what `'a'` should be to make it a real programming language example. Give a leftmost derivation to show that the sentence `aa+a*` can be generated by this grammar, and draw the corresponding _parse tree_. **(2 marks)**

```
⟨S⟩ → ⟨S⟩ ⟨S⟩ + | ⟨S⟩ ⟨S⟩ * | a
```

---

**(b)** Write a strict _leftmost reverse derivation_ to show that the sentence `aaa+a*` _cannot_ be generated by the grammar in part (a). Next, write a _mixed_ reverse derivation, trying to go as far as possible… In both cases, indicate precisely how it stops and what the syntax error is. Explain briefly whether, in general, one approach is better than the other. **(3 marks)**

> [!success]- Solution
> **Strict leftmost:**
> 
> ```
> aaa+a*
> ⟨S⟩aa+a*
> ⟨S⟩⟨S⟩a+a*
> ⟨S⟩⟨S⟩⟨S⟩+a*   ← STUCK. Strict leftmost tries to reduce the leftmost ⟨S⟩⟨S⟩ but no rule matches ⟨S⟩⟨S⟩ alone (need + or * after). Can't skip ahead → FAIL.
> ```
> 
> **Mixed reverse derivation** (flexible — can reduce anywhere):
> 
> ```
> aaa+a*
> ⟨S⟩⟨S⟩⟨S⟩+⟨S⟩*       (replace all a's with ⟨S⟩)
> ⟨S⟩⟨S⟩⟨S⟩*             (reduce ⟨S⟩⟨S⟩+ → ⟨S⟩ using 2nd and 3rd)
> ⟨S⟩⟨S⟩                  (reduce ⟨S⟩⟨S⟩* → ⟨S⟩)
> FAIL — ⟨S⟩⟨S⟩ cannot reduce to ⟨S⟩. No rule produces just ⟨S⟩⟨S⟩.
> ```
> 
> **Which is better?** Mixed gets further (reaches `⟨S⟩⟨S⟩` and pinpoints the real error — one extra operand). Strict leftmost gets stuck earlier at a less informative point. So mixed is generally better for finding the actual syntax error.
> 
> **The error:** There are 3 operands (`aaa`) but only 2 operators (`+*`). In postfix, n operands need n−1 operators.


---

**(c)** Is the above grammar ambiguous? Justify clearly why, or not. Consider the sentence `aaa+*` as example to illustrate your explanations. **(2 marks)**

> [!success]- Solution
> Not ambiguous. One parse tree. In postfix/prefix, the operator's fixed position tells you exactly which operands it takes. No choice = no ambiguity.
> ![image-45.png|400x270](/img/user/1%20-%20MW%20CMP321/img/image-45.png)


---

### Exam 14: Question 4 — English Grammar Ambiguity

**(a)** Consider the BNF grammar below (part of the English language). Draw _two parse trees_ to show that the sentence "I saw an elephant in my pyjamas" has _two possible interpretations_, and that the grammar is ambiguous. Rephrase the sentence slightly, twice, to _make each interpretation clear_. **(3 marks)**

```
⟨S⟩   → ⟨NP⟩ ⟨VP⟩
⟨PP⟩  → ⟨P⟩ ⟨NP⟩
⟨NP⟩  → ⟨D⟩ ⟨N⟩ | ⟨D⟩ ⟨N⟩ ⟨PP⟩ | 'I'
⟨VP⟩  → ⟨V⟩ ⟨NP⟩ | ⟨VP⟩ ⟨PP⟩
⟨D⟩   → 'a' | 'an' | 'my' | 'the' | 'your'
⟨N⟩   → 'banana' | 'elephant' | 'mouse' | 'pyjamas'
⟨V⟩   → 'found' | 'heard' | 'saw' | 'shot'
⟨P⟩   → 'in' | 'inside' | 'outside'
```

---

**(b)** Rewrite the grammar below to make it _unambiguous_. **(2 marks)**

```
⟨num⟩ → ⟨bin⟩ ⟨num⟩ | ε
⟨bin⟩ → 01 | ⟨bin⟩ 1 | 0 ⟨bin⟩ 1
```

> [!success]- Solution
> The fix is to **remove one** of the two conflicting rules. Drop `⟨bin⟩ 1`:
> ```
> ⟨num⟩ → ⟨bin⟩ ⟨num⟩ | ε
> ⟨bin⟩ → 01 | 0 ⟨bin⟩ 1
> ```

---

### Exam 14: Question 5 — BNF to EBNF

**(a)** Consider the language defined by the BNF grammar below. Describe in plain English what its _sentences_ consist of. Write the equivalent EBNF, showing the conversion steps. **(3 marks)**

```
⟨S⟩ → ⟨A⟩ b | ⟨A⟩ b ⟨C⟩
⟨A⟩ → a | a ⟨A⟩
⟨C⟩ → c | ⟨C⟩ c
```

> [!success]- Solution
> ```
> <S> -> 
> Conversion steps
> ⟨A⟩ b | ⟨A⟩ b ⟨C⟩
> <A> b [<C>]  <-- make C optional part
> {a}+ b [<C>] <-- simplify all of <A>
> {a}+ b [{c}+] <-- simplify all of <C>
> {a}+ b {c}  <-- [{c}+] = {c} simplified since optional = 0 and {c}+ = 1 or more
> 
> Final
> {a}+ b {c}
> ```

> **Note:** The regex part of the original question is ❌ not M1 scope. Part (b) format specifier regex also ❌.

---

### Exam 14: Question 6 — Roman Numeral Attribute Grammar

**(a)** The following rule set defines a simple BNF grammar for Roman numerals of value less than 1000. Complete the _semantic rules_ that specify how the `val` attribute is computed. Note that c=100, l=50, x=10, v=5, i=1, and symbol values are added except: i before v or x indicates one less (e.g., iv is 4) and x before l or c indicates ten less (e.g., xc is 90). Use the semantic rules to _evaluate_ the Roman numeral `xcvii`, showing clearly all the calculation steps. **(3 marks)**

```
⟨S⟩ → x⟨T⟩⟨U⟩
⟨S⟩ → l⟨X⟩
⟨S⟩ → ⟨X⟩
⟨T⟩ → c
⟨T⟩ → l
⟨U⟩ → i⟨Y⟩
⟨U⟩ → v⟨I⟩
⟨U⟩ → ⟨I⟩
⟨X⟩[1] → x⟨X⟩[2]
⟨X⟩ → ⟨U⟩
⟨Y⟩ → x
⟨Y⟩ → v
⟨I⟩[1] → i⟨I⟩[2]
⟨I⟩ → ε
```

> [!success]- Solution
> ```rules
> ⟨S⟩ → x⟨T⟩⟨U⟩      <S>.val=<T>.val+<U>.val-10
> ⟨S⟩ → l⟨X⟩        <S>.val=50+<X>.val
> ⟨S⟩ → ⟨X⟩         <S>.val=<X>.val
> ⟨T⟩ → c          <T>.val=100
> ⟨T⟩ → l          <T>.val=50
> ⟨U⟩ → i⟨Y⟩        <U>.val=<Y>.val-1
> ⟨U⟩ → v⟨I⟩        <U>.val=5+<I>.val
> ⟨U⟩ → ⟨I⟩         <U>.val=<I>.val
> ⟨X⟩[1] → x⟨X⟩[2]  <X>[0].val=10+<X>[1].val
> ⟨X⟩ → ⟨U⟩         <X>.val=<U>.val
> ⟨Y⟩ → x          <Y>.val = 10
> ⟨Y⟩ → v          <Y>.val = 5
> ⟨I⟩[1] → i⟨I⟩[2]  <I>[0].val=1+<I>[1].val
> ⟨I⟩ → ε          <I>.val=0
> 
> ```
> 
> ```
> xcvii
> <S>
> x<T><U>  <S>.val=<T>.val+<U>.val-10         <S>.val=100+7-10=97
> xc<U>    <T>.val=100
> xcv<I>   <U>.val=5+<I>.val                  <U>.val=5+2=7
> xcvi<I>  <I>[0].val=1+<I>[1].val            <I>[0].val=2
> xcvii<I> <I>[1].val=1+<I>[2].val            <I>[1].val=1
> xcvii    <I>[2].val=0
> 
> ---
> we will go bottoms up for calculation (synthesized)
> ```

---

	**(b)** The above grammar allows illegal forms such as `xiiii` or `xxxxx`. Add the necessary _attribute/s_, _semantic rule/s_, and _predicate/s_ to ensure that generated sentences contain groups of at most 3 `i` or 3 `x`. Draw a _synthetized, decorated parse tree_ showing that `lviiii` is _not_ a valid Roman numeral. **(4 marks)**



```
attributes
<I>.cnt ∈ {0,1,2,3}
<X>.cnt ∈ {0,1,2,3}

semantic rules
i<I>[2] <- <I>[0].cnt=<I>[1].cnt+1 
ε    <- <I>.cnt=0
⟨U⟩  <- ⟨X⟩.cnt = 0
x<X>[2] <- <X>.cnt=<X>[1].cnt+1


predicates
<I>.cnt <=3
<X>.cnt <=3

```

---

_End of Exam 14 (Final C)_

---

## Exam 15: Appendix — Reconstructed Questions from Student Answers

> **📌 Source:** CMP321_Finals.md — Appendix (S2021.docx, questions reconstructed from student answers)



---

### Exam 15: Palindrome BNF & Attribute Grammar

**(a)** A classmate proposed the following BNF grammar rule for palindromes:

```
⟨palindrome⟩ → ⟨letter⟩ ⟨palindrome⟩ ⟨letter⟩ | ⟨letter⟩ | ''
```

Explain why this grammar is _incorrect_ for defining palindromes. Propose a correct solution using BNF only. Discuss the drawbacks of your approach.

---

**(b)** Design an _attribute grammar_ (attributes, predicates, and semantic rules) that correctly validates palindromes using the original BNF structure from part (a).

---

### Exam 15: Lexical Analyzer vs Parser — Integer Expressions

Given the following tokens for a simple integer expression language:

```
⟨pos-digit⟩  ⟨any-digit⟩  ⟨op⟩  ⟨sign⟩  ⟨int⟩  ⟨digits⟩  ⟨number⟩
```

With the syntax analyzer using `⟨expr⟩`:

**(a)** Determine whether each of the following expressions is _valid_ or _invalid_, showing the tokenization:

```
  I)   -123  +  800
  II)  421  -33  +  7
  III) 1  +  0
```

---

**(b)** Assuming `+` remains in `⟨op⟩` as well as potentially in `⟨sign⟩`, explain the _ambiguity_ the lexical analyzer will encounter and how to resolve it.

---

_End of Exam 15 (Appendix)_

---

## Exam 16: Midterm 1 — Spring 2019

> **📌 Source:** Midterm_1_-_Spring_2019.pdf (5 pages, 1-hour exam, with official solutions)

---

### Exam 16: Question 1 — C vs Python RWR, Type Inference Costs & Orthogonality

**(a)** Characterize and compare precisely the C program on the right with the Python script below in terms of _readability_, _writability_, and _reliability_. **(4 marks)**

```python
print(sum(range(1,66)))   # Python
```

```c
int sum=0, val=1;
while (val < 66)
{ sum += val;
  val += 1; }
print(sum);   // C
```

> **🔁 REDUNDANT:** Same as Exam 8 Q1(c), Exam 11 Q1(a).

---

**(b)** Does the availability of _type inference_ in a programming language increase (↑) or decrease (↓) each cost type below? Circle one arrow for each. **(2 marks)**

| Cost                  | ↑ or ↓ |
| --------------------- | ------ |
| Training programmers  |        |
| Writing programs      |        |
| Compiling programs    |        |
| Executing programs    |        |
| Maintaining programs  |        |
| Program unreliability |        |

> [!success]- Solution
> 
> - **Training programmers**: ↓ — less syntax to learn (no need to memorize type declarations)
> - **Writing programs**: ↓ — shorter code, less typing
> - **Compiling programs**: ↑ — compiler must do extra work to deduce types
> - **Executing programs**: no change (types are resolved at compile-time; same machine code)
> - **Maintaining programs**: ↓ — less code to maintain, fewer type-related changes needed
> - **Program unreliability**: ↑ — type may not be what programmer intended (implicit = less visible); harder to read/understand what type a variable holds

---

**(c)** What does _orthogonality_ refer to in a programming language? Explain clearly using the example of _type conversion in Java_. **(4 marks)**

> **🔁 REDUNDANT:** Same as Exam 8 Q1(d)(i).

---

### Exam 16: Question 2 — Dynamic Typing, Unique Expressions, Slicing & Format

**(a)** Explain exactly what _dynamic typing_ is, in Python, using the two lines of code shown on the right as example. **(2 marks)**

```python
x = 1
x = 'one'
```

> **🔁 REDUNDANT:** Same as Exam 8 Q2(a).

---

**(b)** Indicate briefly what each of the expressions hereafter represents and which are _unique to Python_ i.e., do not exist in C++ and Java. **(3 marks)**

```
"\u0078"     [66,[],]     1+7j     ()     '"'     N//2
```

> **🔁 REDUNDANT:** Overlaps with Exam 8 Q2(c). New additions: `()` empty tuple (unique), `'"'` quotes within quotes without backslash (unique).

> [!success]- Solution
> 
> - `"\u0078"` — unicode symbol/string. Not unique (C++/Java have it).
> - `[66,[],]` — bracket list notation, empty list element, trailing comma. Unique to Python.
> - `1+7j` — complex number class and notation. Unique to Python.
> - `()` — empty tuple notation. Unique to Python.
> - `'"'` — quotes within quotes without backslash. Unique to Python (no char type, so `'` can delimit strings containing `"`).
> - `N//2` — integer/floor division operator. Unique to Python.

---

**(c)** Explain in detail what the following Python statement does exactly and what its output is: **(3 marks)**

```python
'are scary movies worst at night?'[8:24:6]
```

> **🔁 REDUNDANT:** Same as Exam 8 Q2(d).

---

**(d)** Give the arguments to the `format` function below and, accordingly, the _output_ of the following Python statement, or syntax error if any. **(2 marks)**

```python
x,y = 17,5
print('{0}//{1}={2}, {0}%{1}={3}'.format(x,y,*divmod(x,y)))
```

> **🔁 REDUNDANT:** Same as Exam 9 Q2(d).

---

### Exam 16: Question 3 — lsub Function & Square Class

**(a)** Code the Python function below that replaces the elements from `alist` in the range `m..n` by the elements from the given `newlist`. **(3 marks)**

> [!success]- Solution
> 
> ```python
> def sub(alist, m, n, newlist):
>     alist[m:n] = newlist
> ```
> 
> No need to check for bounds — errors will be silently ignored by Python slicing.
> OR : `alist[m:n] = newlist[:]`

> **🔁 REDUNDANT:** Simpler variant of Exam 8 Q3(a) / Exam 11 Q2(a).

---

**(b)** Write a minimal Python `Square` class so that the following code works as specified. All attributes should be "private" and the width should always be an int value. Use standard Python coding and naming practices. **(5 marks)**

```python
s1 = Square()          # creates a new square of default width 1
s2 = Square(10)        # creates a new square with custom width (10)
print(len(s2))         # prints the square's current width
s3 = Square('ten')     # exception caught, error message printed
```

> **🔁 REDUNDANT:** Same as Exam 8 Q4(a) / Exam 9 Q4(a) / Exam 11 Q4(a). Default width = 1 here.

> [!success]- Solution
> 
> ```python
> class Square:
>     def __init__(self, width=1):
>         try:
>             self.__width = int(width)
>         except ValueError:
>             print("error: width must be a number")
>     def __len__(self):
>         return self.__width
> ```

Alternative Solution
> [!success]- Solution
> ```python
> class Square:
>  def __init__(self, width=1): 
>   if (type(width) is not int): raise TypeError("Value is not of type int. ERROR.") 
>   self._width=width
>    
>  def __len__(self):
>   return self._width 
> ```

---

### Exam 16: Question 4 — Average Length & Sieve Comprehension

**(a)** Write one Python expression (not a comprehension) that will calculate the average length of all lists contained in a dictionary `d`. **(2 marks)**

```
e.g., d = {'A':[1,2], 'B':[3], 'C':[4,5,6]} → 2
```

> **🔁 REDUNDANT:** Same as Exam 6 Q2(b), Exam 8 Q5(a), Exam 11 Q5(b).

> [!success]- Solution
> `sum(map(len, d.values())) / len(d)`

---

**(b)** Explain what the Python comprehensions below do, i.e., what `x` and `y` will contain, respectively. What would be different if we used `{}` instead? **(5 marks)**

```python
x = [j for i in range(2, 5) for j in range(i*2, 50, i)]
y = [n for n in range(2, 50) if n not in x]
```

> [!success]- Solution
> The two nested loops generate a list `x` of all multiples of 2, 3, and 4 (starting from `i*2` up to 49, stepping by `i`).
> 
> Using `{}` instead of `[]` would create a **set**, removing duplicates — more efficient for the `not in` check.
> 
> `y` is therefore a list of numbers from 2–49 that are NOT multiples of 2, 3, or 4. This is an approximation of the **Sieve of Eratosthenes** for finding primes, though the range should have been `range(2, 8)` to get only true primes (as-is, it also includes squares of 5 and 7: 25 and 49).
> 
> Note: `x` contains duplicates (e.g., 12 appears as a multiple of both 2 and 3). Using a set `{}` would eliminate these and make the membership test O(1) instead of O(n).

My sol:
> [!success]- Solution
> x = [expression | outer loop | inner loop]
> 
> 
> | i   | j                                |
> | --- | -------------------------------- |
> | 2   | 4<br>6<br>8<br>10<br>...<br>48   |
> | 3   | 6<br>9<br>12<br>15<br>...<br>48  |
> | 4   | 8<br>12<br>16<br>20<br>...<br>48 |
> 
> x will contain numbers divisible by 2 (>=4 and <=48), numbers divisible by 3 (>=6 and <=48), numbers divisible by 4 (>=8 and <=48).
> 
> y = [expression | loop | condition]
> 
> 
> | n   |
> | --- |
> | 2   |
> | 3   |
> | 4   |
> | ... |
> | 49  |
> 
> y= [2,3,5,7,11,...,49]
> meaning y will only contain the values that do not occur in x (i.e. numbers divisible by 2 (>=4 and <=48), numbers divisible by 3 (>=6 and <=48), numbers divisible by 4 (>=8 and <=48)
> 
> 
> if we used {} it would perform set comprehensions instead. Meaning all the duplicates in x would be removed (ex. 48 will only appear once in list). However, this does not affect y since y only needs the number to not occur in x at least once to exclude it. It also optimizes it since the `not in` check is O(1) on set vs O(n) on list.

Alternative solution:

> [!success]- Solution
> j in range(4,50,2)
> j in range(6,50,3)
> j in range(8,50,4)
> 
> [4,6,...,48] (contains all numbers divisible by 2 from 4 to 49)
> [6,9,...,48] (contains all numbers divisible by 3 from 6 to 49)
> [8,12,...,48] (contains all numbers divisible by 4 from 8 to 49)
> but combined in one list with repeated values [4,6,...,48, 6,9,...,48, 8,12,...,48]
> 
> if it was {} -> set notation. then it will just be all unique numbers (no duplicate) divisible by 2,3,4 from 4 to 49, 6 to 49, 8 to 49 respectively.
> 
> y wouldn't change regardless of notation since if there is duplicate or not its still excluded. Only difference is now since it's set the time complexity is faster since set operations are faster.
> 
> y will contain numbers from 2 to 49 that aren't in the list (or set for part 2) of x.
> Ex. [2,3,5,7,11,...,49]


---

### Exam 16: Question 5 — Tail-Recursive lzip, map-based zip & Efficiency ⭐

**(a)** Write a _tail recursive_ Python function that iterates over two lists in parallel and returns a list of tuples comprising one item from each list (like `zip`). The lists may differ in length. **(4 marks)**

```python
# lzip([1,2,3,4,5], ['i','ii','iii','iv'])
# -> [(1, 'i'), (2, 'ii'), (3, 'iii'), (4, 'iv')]
```

> [!success]- Solution
> 
> ```python
> def lzip(l1, l2, l=[]):
>     if not l1 or not l2: return l
>     return lzip(l1[1:], l2[1:], l + [(l1[0], l2[0])])
> ```
> 
> Uses tail recursion: result accumulates in `l`, and the recursive call is the last operation. Stops when either list is exhausted (handles different lengths).

> [!success]- Alternative Solution
> ```python
> def lzip(lst, lst2, acc = []):
>  if (not lst or not lst2):
>   return acc
>  
>  return lzip(lst[1:], lst2[1:], acc+[(lst[0],lst2[0])])
> ```

---

**(b)** Re-write `zip` using only `map` and a lambda expression. **(2 marks)**

> [!success]- Solution
> 
> ```python
> def zip(l1, l2):
>     return map(lambda x, y: (x, y), l1, l2)
> ```
> 
> `map` with two iterables passes one element from each to the lambda in parallel.

---

**(c)** Is the recursive version in part (a) as efficient as the built-in `zip` function? What about the `map` version in part (b)? Explain briefly. **(3 marks)**

> [!success]- Solution
> The built-in `zip` returns an **iterator** (lazy), so items are generated one-by-one and only when needed — saving both memory and computation time.
> 
> The recursive `lzip` generates the **entire list** upfront (eager), which is bad for large inputs — it consumes O(n) memory immediately. Also, `l1[1:]` creates a new list copy each call → O(n²) total.
> 
> The `map` version also creates an **iterator** (lazy), and is therefore as efficient as `zip` itself.

> [!success]- Alternative Solution
> "The recursive lzip is much less efficient than built-in zip. (1) zip is lazy — returns an iterator generating pairs on demand, using O(1) memory; lzip is eager, building the full list upfront. (2) l1[1:] slicing creates a list copy each recursive call → O(n²) memory and time. The map version is also lazy (returns an iterator), so it's as efficient as built-in zip."

---

### Exam 16: Question 6 — Multiple Choice (Abstraction, Features, Type Check, MI)

In each of the following, highlight the only correct response. **(6 marks)**

**1.** It is important for a programming language to support abstraction, primarily because of:

- (A) Readability
- (B) Writability
- (C) Program cost
- (D) Reliability
- (E) None of the above

> [!success]- Solution
> **Answer: B** — Abstraction primarily improves writability by allowing programmers to express complex ideas concisely.

---

**2.** Some of the notable features of the Python programming language include:

- (A) Dynamic typing
- (B) Garbage collection
- (C) High-order functions
- (D) B and C
- (E) A, B, and C

> [!success]- Solution
> **Answer: E** — Python has all three: dynamic typing, garbage collection, and higher-order functions.

---

**3.** Which statement below is the correct way to ensure that `s` is a string?

- (A) `if s is not type(str): raise TypeError`
- (B) `if type(s) is not type(str): raise TypeError`
- (C) `if type(s) is not str: raise TypeError`
- (D) `if s.type() is not str: raise TypeError`
- (E) `if s.__type__ is not str: raise TypeError`

> [!success]- Solution
> **Answer: C** — `type(s)` returns the type of `s`, and `str` is the string class itself. Comparing with `is` checks identity. Note: `isinstance(s, str)` is more Pythonic, but C is the correct choice among these options.

---

**4.** Does Python allow for multiple inheritance?

- (A) Yes but only if the base classes have different methods
- (B) Yes but only if the base classes have the same methods
- (C) Yes but methods are inherited from the first matching base class only
- (D) Yes but methods are inherited from the last matching base class only
- (E) No it does not because of the "diamond of death" problem

> [!success]- Solution
> **Answer: C** — Python uses the **MRO (Method Resolution Order)** via C3 linearization. When multiple base classes have the same method, the version from the **first** parent class (left to right) in the class definition is used.

---

_End of Exam 16 (Midterm 1 — Spring 2019)_

---

## Exam 17: Final Exam — Spring 2021

> **📌 Source:** S2021Final.pdf (14 pages, 8 questions)

---

### Exam 17: Question 1 — Increment Operators & Orthogonality Benefits/Drawbacks

**(a)** In each case below, compare the given versions of a programming language feature in terms of _readability_, _writability_, and _reliability_. **(6 marks)**

**(i)** Increment operator: `count=count+1` vs. `count++` vs. having _both_

> [!success]- Solution
> 
> - **Readability**: `count=count+1` is most readable — fully explicit about what's happening. `count++` is concise but requires knowing the convention. Having **both** is slightly worse since the reader must know two syntaxes for the same operation.
> - **Writability**: `count++` is most writable — shortest to type. `count=count+1` is longer. Having **both** maximizes writability (programmer picks preferred form).
> - **Reliability**: `count=count+1` is most reliable — no ambiguity. `count++` can be confused with `++count` (pre vs post increment), and having **both** `count=count+1` and `count++` introduces redundancy which can create inconsistencies and confusion (two ways to do same thing → unorthogonal).

**(ii)** Boolean vs. using int as Boolean: `count=true` vs. `count=1`

> [!success]- Solution
> 
> - **Readability**: `count=true` is more readable — it's clear the intent is Boolean. `count=1` is ambiguous — is it a number or a Boolean flag?
> - **Writability**: `count=1` is slightly more writable (shorter), but the difference is negligible. `count=true` may require importing/defining a Boolean type in some languages.
> - **Reliability**: `count=true` is more reliable — type system can catch misuse (e.g., accidentally doing arithmetic on a Boolean). `count=1` allows mixing arithmetic and Boolean logic silently (e.g., `count = count + 2` on a "Boolean" — no error raised but logically wrong).

---

**(b)** Give _one benefit_ and _one drawback_ of having strict _orthogonality_ in a programming languages. Illustrate each case with an example. **(4 marks)**

> [!success]- Solution
> **Benefit**: Consistency and predictability. If a feature works one way, it works the same way everywhere. Example: In Python, assignment `X=Y` works for all types because everything is an object reference (orthogonal). In Java, `X=Y` works differently for primitives vs objects (unorthogonal), which is confusing.
> 
> **Drawback**: Can lead to absurd or meaningless combinations that the language must still allow. Example: If a language is fully orthogonal with data types and operators, then `"hello" - 3` or `true / false` would need to be valid expressions. Strict orthogonality can sacrifice safety and common sense for the sake of consistency. ALGOL 68 is a well-known example where extreme orthogonality made the language overly complex and hard to learn.

---

### Exam 17: Question 2 — Templates, range() & Memoized Fibonacci

**(a)** Explain why the Python language does _not_ need templates. **(3 marks)**

> [!success]- Solution 
> Templates (C++) / Generics (Java) exist because those languages are statically typed — a function like `swap(a, b)` needs to know the types of `a` and `b` at compile time, so you need `template<typename T>` to make it work for any type.
> 
> Python doesn't need templates because of **dynamic typing**: variables are references to objects, and the type is associated with the object at runtime, not the variable. A Python function like `def swap(a, b): return b, a` works for **any** type without any template/generic syntax. The same function handles ints, strings, lists, etc. — this is known as **duck typing** ("if it quacks like a duck...").
> 
> Additionally, Python containers (lists, dicts, etc.) are **heterogeneous** — they can hold objects of any type — so there's no need for `vector<int>` vs `vector<string>`.

---

**(b)** Explain what `range(x,y,z)` does in Python 3 and write a simple statement to produce the output: `[20,16,12,8,4,0,-4,-8]`. **(3 marks)**

> [!success]- Solution 
> `range(x, y, z)` creates a lazy sequence of numbers starting at `x`, ending before `y`, with step `z`. It returns a range object (iterator), not a list.
> 
> ```python
> list(range(20, -9, -4))
> ```
> 
> Starts at 20, steps by -4, stops before -9 (last value is -8). Wrapped in `list()` to produce the actual list.

---

**(c)** Write a Python-style Fibonacci function that implements the classic recurrence formula i.e., `fib(n)=fib(n-1)+fib(n-2)` with `fib(0)=0` and `fib(1)=1`, while calculating each value only once. Hint: use a dictionary. **(6 marks)**

> [!success]- Solution
> 
> ```python
> def fib(n, memo={0: 0, 1: 1}):
>     if n not in memo:
>         memo[n] = fib(n-1) + fib(n-2)
>     return memo[n]
> ```
> 
> Uses **memoization** via a dictionary default argument (which persists across calls since default mutable arguments are created once). The dictionary caches previously computed values, ensuring each Fibonacci number is calculated only once → O(n) time instead of O(2ⁿ) for naive recursion.
> 
> Alternative (explicit global dict):
> 
> ```python
> cache = {0: 0, 1: 1}
> def fib(n):
>     if n not in cache:
>         cache[n] = fib(n-1) + fib(n-2)
>     return cache[n]
> ```

---

### Exam 17: Question 3 — Comprehension/HOF Rewrite & Fibonacci via reduce

**(a)** Rewrite the `for` loop below **(i)** using a _comprehension_ and **(ii)** using classic _higher-order functions_ i.e., map, filter, reduce, etc. **(5 marks)**

```python
lst, res = ['10','7','12','4','5','11'], []
for n in lst:
    if int(n)%2==1: res += [int(n)]
```

> [!success]- Solution 
> **(i) Comprehension:**
> 
> ```python
> res = [int(n) for n in lst if int(n) % 2 == 1]
> ```
> 
> **(ii) Higher-order functions:**
> 
> ```python
> res = list(filter(lambda n: n % 2 == 1, map(int, lst)))
> ```
> 
> First `map(int, lst)` converts all strings to ints, then `filter` keeps only the odd ones.

Alternative for ii)
> [!success]- Solution
> ```python
> res = list(
>              map(int,
>                        filter(lambda x: int(x)%2==1, lst) ))
> ```

---

**(b)** Consider the code below and indicate what `fun(N)` calculates. Explain briefly the code logic, and especially what each step of `reduce` does exactly. Trace the example of `fun(6)` to illustrate your answer in detail. **(7 marks)**

```python
fun = lambda n: reduce(lambda x,n: (x[1], x[0]+x[1]),
                       range(n), (0,1)) [0]
```

> **🔁 REDUNDANT:** Same as Exam 5 Q3(b). See Exam 5 for solution.

> [!success]- Solution
> list(map(int(x), filter(lambda n: int(n)%2\=\=1, ['10','7','12','4','5','11'] )))

---

### Exam 17: Question 4 — Reversed: Slicing, Iterator & Generator

**(a)** Indicate what the following Python statement does, and _why_ it is very inefficient. What should `data` be for this code to work? **(3 marks)**

```python
for item in data[::-1] : print(item)
```

**(b)** Code the _iterator class_ `X` below so that the following `for` loop is equivalent to the above in part (a), except it is now very efficient. Do not use the built-in `reversed` function. **(7 marks)**

```python
for item in X(data) : print(item)

class X:
    def __init__(
```

**(c)** Write a _generator function_ `X` that can be used instead of the iterator. **(4 marks)**

> **🔁 REDUNDANT:** Same as Exam 5 Q6.

---

### Exam 17: Question 5 — Regular Expressions

**(a)** Describe, in normal English (not programming lingo), exactly _what kind of sentences_ match each of the following regular expressions. **(7 marks)**

**(i)** `(?:[0-9a-fA-F]{2})+`

**(ii)** `(0|(1(01*0)*1))*`

---

**(b)** Give a _regular expression_ matching integers in Python, which contain one or more digits, and may also contain underscore characters (for readability). The first digit cannot be 0. Any underscore must be preceded and followed by at least one digit. **(5 marks)**

Examples: `1_234`, `33_76_48_32`, or `971_6_3521_8`

---

**(c)** Explain what the regular expressions `"t.*o"` and `"t.*?o"` will match exactly and why. Show the result/s of applying them both (via `findall`) to the sentence `"tea for two and two for tea"`. **(4 marks)**

---

> **Note:** Q5 is entirely regex (Week 13) — ❌ not M1 scope.

---

### Exam 17: Question 6 — Ambiguous C++ Grammar & Resolution

The BNF grammar rules below define C++ output statements, where `⟨ostream⟩` can be any output stream variable e.g., `cout`, and `⟨string⟩` represents any valid string object, while `⟨int⟩` denotes a literal integer.

```
⟨xpr⟩ → ⟨xpr⟩ '<<' ⟨xpr⟩ | ⟨obj⟩
⟨obj⟩ → ⟨ostream⟩ | ⟨string⟩ | ⟨int⟩
```

**(a)** Explain why this grammar is _ambiguous_. Show two different _derivations_ (left, right, or mixed) for the following sentence: `cout << "n=" << 4`. **(6 marks)**

> **🔁 REDUNDANT:** Same grammar as Exam 2 Q3(d). See Exam 2 for the ambiguity explanation and two parse trees. This variant asks for **derivations** instead of parse trees.

---

**(b)** Resolve the ambiguity by making _one change_ to the above grammar. Justify. Show the resulting _derivation_ for the same sentence as in part (a). **(4 marks)**

> [!success]- Solution
> The issue is that `⟨xpr⟩ → ⟨xpr⟩ '<<' ⟨xpr⟩` is both left- and right-recursive, allowing two different parse structures.
> 
> **Fix:** Force left-associativity by replacing the recursive rule:
> 
> ```
> ⟨xpr⟩ → ⟨xpr⟩ '<<' ⟨obj⟩ | ⟨obj⟩
> ```
> 
> Now the right side of `<<` must always be an `⟨obj⟩` (terminal), not another `⟨xpr⟩`. This forces left-to-right grouping (left-associativity), which matches C++ semantics where `cout << "n=" << 4` means `(cout << "n=") << 4`.
> 
> **Derivation:**
> 
> ```
> ⟨xpr⟩
> → ⟨xpr⟩ << ⟨obj⟩
> → ⟨xpr⟩ << ⟨obj⟩ << ⟨obj⟩
> → ⟨obj⟩ << ⟨obj⟩ << ⟨obj⟩
> → cout << ⟨obj⟩ << ⟨obj⟩
> → cout << "n=" << ⟨obj⟩
> → cout << "n=" << 4
> ```
> 
> Only one derivation is possible now → grammar is unambiguous.

---

### Exam 17: Question 7 — Palindrome BNF & Attribute Grammar

**(a)** State why the following BNF grammar for palindromes (words that are the same in reverse e.g., "noon" or "radar") is _incorrect_. Show how it can be fixed by rewriting the BNF rules. Point out the drawbacks of this approach. **(5 marks)**

```
⟨palindrome⟩ → ⟨letter⟩ ⟨palindrome⟩ ⟨letter⟩ | ⟨letter⟩ | ''
⟨letter⟩     → a | b | ... | z | A | B | ... | Z
```

**(b)** Solve the problem in part (a) by adding _attribute(s)_, semantic _rule(s)_ and _predicate(s)_ as necessary, instead of rewriting the BNF rules. **(5 marks)**

> **🔁 REDUNDANT:** Same as Exam 15 Appendix A1. This version provides the full original question text.

---

### Exam 17: Question 8 — Lexical Analyzer vs Syntax Analyzer

Consider the simple BNF grammar for integral numbers shown below.

```
⟨expr⟩      → ⟨int⟩ ⟨op⟩ ⟨int⟩ | ⟨int⟩ ⟨op⟩ ⟨expr⟩       #1
⟨int⟩       → ⟨number⟩ | ⟨sign⟩ ⟨number⟩                   #2
⟨op⟩        → + | *                                         #3
⟨sign⟩      → -                                             #4
⟨number⟩    → ⟨any-digit⟩ | ⟨pos-digit⟩ ⟨digits⟩           #5
⟨digits⟩    → ⟨any-digit⟩ | ⟨any-digit⟩ ⟨digits⟩           #6
⟨any-digit⟩ → 0 | ⟨pos-digit⟩                              #7
⟨pos-digit⟩ → 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9          #8
```

**(a)** Explain which of rules #1–8 are used by the _lexical analyzer_ and which are used by the _syntax analyzer_, respectively, and how. List out the tokens and give a brief definition of each, in words (based on the grammar). **(6 marks)**

> [!success]- Solution
> **Lexical analyzer** uses rules #2–#8 (lower-level rules that define individual tokens):
> 
> - Rules #5–#8 define the structure of `⟨number⟩` (sequences of digits)
> - Rule #4 defines `⟨sign⟩` (the `-` character)
> - Rule #3 defines `⟨op⟩` (operators `+` and `*`)
> - Rule #2 combines sign and number into `⟨int⟩`
> 
> **Syntax analyzer** uses rule #1 (the high-level structure):
> 
> - Rule #1 defines `⟨expr⟩` — how integers and operators combine into expressions
> 
> **Tokens:**
> 
> - `⟨int⟩` — a signed or unsigned integer (e.g., `-123`, `800`, `7`)
> - `⟨op⟩` — an arithmetic operator (`+` or `*`)

---

**(b)** For each sentence below, give the output of the lexical analyser (i.e., a list of lexemes and their tokens), show the recognition work done accordingly by the syntax analyser, and indicate the outcome i.e., whether the sentence is valid or, if not, which error is detected. **(6 marks)**

**(i)** `-123+800`

> [!success]- Solution
> Lexer output: `⟨int:-123⟩ ⟨op:+⟩ ⟨int:800⟩` Parser: `⟨expr⟩ → ⟨int⟩ ⟨op⟩ ⟨int⟩` ✓ Valid.

**(ii)** `421-33+7`

> [!success]- Solution
> Lexer output: `⟨int:421⟩` then `-` ... but `-` is `⟨sign⟩`, not `⟨op⟩`. So lexer produces: `⟨int:421⟩ ⟨int:-33⟩ ⟨op:+⟩ ⟨int:7⟩` Parser: expects `⟨int⟩ ⟨op⟩ ⟨int⟩` but gets `⟨int⟩ ⟨int⟩ ...` → **Syntax error**: two consecutive `⟨int⟩` tokens with no operator between them. (The issue: `-` is only defined as `⟨sign⟩`, not as an `⟨op⟩`.)

**(iii)** `1+06`

> [!success]- Solution
> Lexer: `1` → rule #5 first option: `⟨any-digit⟩` → `⟨number⟩` → `⟨int:1⟩`. Then `+` → `⟨op:+⟩`. Then `06`: first digit is `0`, so by rule #5, `⟨number⟩ → ⟨any-digit⟩` gives just `0`. But then `6` is left over — it can't start a new token without an operator. Alternative: `06` could be `⟨any-digit⟩ ⟨digits⟩` via rule #6, but rule #5 requires `⟨pos-digit⟩ ⟨digits⟩` for multi-digit numbers (no leading zeros). Result: **Lexical error** — `06` is not a valid `⟨number⟩` (leading zero not allowed for multi-digit numbers).

---

**(c)** Explain the issue created if we change rule #4 to: `⟨sign⟩ → + | -`. Think of a possible solution and give the idea briefly. **(4 marks)**

> [!success]- Solution
> If `+` is both an `⟨op⟩` (rule #3) and a `⟨sign⟩` (rule #4), the lexical analyzer faces **ambiguity**: when it sees `+`, it cannot determine whether it is an operator between two integers or a sign prefix for the next integer.
> 
> For example, `1+2` could be tokenized as:
> 
> - `⟨int:1⟩ ⟨op:+⟩ ⟨int:2⟩` (correct: addition)
> - `⟨int:1⟩ ⟨int:+2⟩` (wrong: two consecutive integers)
> 
> **Possible solution**: Use **context** — if the previous token was an `⟨int⟩`, then `+`/`-` is an `⟨op⟩`; if the previous token was an `⟨op⟩` or it's the start of the expression, then `+`/`-` is a `⟨sign⟩`. This requires the lexer to maintain state (look at the previous token), making it context-sensitive rather than purely context-free.

---

_End of Exam 17 (Final Exam — Spring 2021)_

---
