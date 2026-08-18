# Book-style worked examples

These are concise, book-style model answers — one per question type — based on the
approach in *Cracking the PM Interview*. Use them when the user is stuck on a step
and wants to see what a strong answer looks like, or asks for a full model answer.
Adapt the structure to whatever question the user is actually practicing; don't
just recite these verbatim.

The constant across all three: **identify the users/customers → identify the use
cases → solve for the use cases, in a structured way (CUF).**

---

## Type 1 — Design a Product

**Q: "Google Maps is launching a version for schools. How would you design it?"**

**a. Clarifying questions.** Is this for colleges, high schools, or middle schools?
Just students, or faculty too? Free or paid? — Assume: colleges, students only.

**b. Structure.** "I'll identify the users and customers, list their use cases,
check how today's products serve those use cases, then propose a design."

**c. Users / customers.** Users are students. If paid, customers could be the
students themselves or the school administration.

**d. Use cases.** Locate academic buildings (campuses can be spread across a city),
find offices inside buildings (a floor-by-floor view), check building/office hours,
find events (exams, free food, RSVP), gauge foot traffic across campus.

**e. How well do current products serve this?** Google/Apple/Baidu Maps give a
macro city view and don't cater to a single campus's interior or community.

**f. Design / improvements.** Gate access per college via college email login (like
school Gmail), so students of college XYZ only see XYZ's map. Let students search
for a building, professor, or office. Tap a building for a per-floor blueprint view.
Surface room/office info. Let the student body create campus events with RSVP.
Show general campus traffic (easy outdoors, hard floor-by-floor).

**g. Wrap up.** A campus-scoped, login-gated map whose core value is interior
navigation + a campus events layer — the things general maps don't do.

---

## Type 2 — Improve a Product

**Q: "What would you change about a supermarket to make it better for college
students?"** (We're told the customers are college students.)

**a. Goal (and user).** A supermarket's goal is to let customers buy quality
products they need at reasonable prices. Use cases for college students: groceries,
some furniture, school items, and (sometimes unknowingly) things not allowed in
dorms.

**b. Problems it faces.** Deals are cluttered and hard to navigate, and many shown
deals are expired. Students struggle to find healthy options because nutrition info
isn't surfaced.

**c. How to solve.** A mobile app or Slack channel pushing only valid deals; deals
tied to the student ID; clear signposting of what is/isn't dorm-allowed; products
sortable by price and/or quality; a "most popular with students" list (helps
international/new students); delivery to dorms.

**d. How to implement.** Partner with the college to run the communication channel
(the school is responsible for student welfare and sets dorm rules), and tie deals
to the existing student ID system.

**e. How to validate.** Track app usage, message open rates, coupons redeemed per
week/month, weekly student footfall, and number of dorm deliveries — compare over
time to gauge whether the changes worked.

---

## Type 3 — Favorite Product

**Q: "What's your favorite business tool? Why?"** (Example pick: Slack.)

**a. Problems it solves.** Faster communication, more effective collaboration, makes
keeping up with important messages less of a chore, and surfaces what's being
discussed across a company.

**b. How it accomplishes that / what makes it neat.** Instant messages instead of
email, instant document sharing, organized channels, searchable history and indexed
files, integrations (Drive, Calendar, RSS), reminders, and cross-org communication.
Smart use of ML/NLP to personalize and rank what matters. Together it acts like a
ruthlessly organized assistant that keeps you briefed on only the salient events.

**c. Compared with alternatives.** Webex Teams, Workplace, Microsoft Teams have
large existing user bases, but Slack is more focused and more functional — part of
why it has strong daily active usage.

**d. How I'd improve it.** Better threading to keep topics coherent, better search,
finer control over chat retention/security, a "do not disturb while focused" mode,
and NLP-generated conversation summaries / topic and priority detection.
