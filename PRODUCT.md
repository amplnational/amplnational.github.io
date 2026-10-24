# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Three audiences, weighted roughly equally (confirmed):

- **Students joining:** Muslim students in the UC system deciding whether to join their campus chapter or attend an event. Membership is free and open to all students.
- **Chapter founders:** students at campuses without AMPL who want to start a chapter. The site says AMPL "will support you every step of the way."
- **Mentors and partners:** practicing attorneys, policymakers and public servants deciding whether to speak, sponsor or partner, or to join the interest list for the mentorship program, which hasn't launched yet.

There is also a fourth, private audience: **chapter officers and AMPL National board members**, who use the Chapter Portal (`portal.html`) to manage their chapter.

## Product Purpose

AMPL (Association of Muslims in Politics and Law) builds a home for Muslims in policy and law. It works through three pillars:

- **Education:** workshops, panels and speaker series on legal systems and policy.
- **Mentorship:** connecting students with practicing Muslim attorneys, policymakers and public servants.
- **Advocacy:** training members to engage with campus policy and state legislation.

The public site exists to get each audience to act: join a chapter, start a chapter, or mentor or partner. The portal exists so chapters can run their operations with AMPL National: announcements, resources, chapter profiles, event reports, and finances, including budget requests and approvals.

## Positioning

AMPL is a student-founded network across the University of California system. It started at UC San Diego. Each chapter is an independent student organization at its university, united by a shared mission and national identity. Its stance is that "representation is not just symbolic — it changes outcomes."

## Operating Context

- **Public site:** a single page (`index.html`) with in-page views for Home, About, Chapters (with a California map of chapter locations), Events, Get Involved and Contact.
- **Contact form:** submissions go through Formspree.
- **Chapters:** six active chapters at UC San Diego, UC Berkeley, UC Irvine, UCLA, UC Santa Cruz and UC Davis.
- **Chapter Portal:** `portal.html`, backed by Firebase Auth and Firestore. Access rules live in `firestore.rules`, and setup steps are in `PORTAL_SETUP.md`. There are three roles: pending, chapter officer, and National admin.
- **Contact details:** amplnational@gmail.com and @amplnational on Instagram.

## Capabilities and Constraints

- Hosted on GitHub Pages at amplnational.com (custom domain set in `CNAME`). The site is static, with no build step or server code. Anything dynamic must go through a client-side service such as Formspree or Firebase.
- The user maintains the site personally, with AI help. Keep it editable as plain HTML, CSS and JS.
- Event listings are hard-coded in `index.html`. Whether these events are current is unconfirmed.
- **Open decision:** the hero promises "real placements in law and policy," but there is no placement evidence on hand (see Evidence on Hand). This line needs either evidence or a rewrite.

## Brand Commitments

- **Name:** Association of Muslims in Politics and Law, written "AMPL" or "AMPL." with a trailing period in the wordmark.
- **Logo:** `images/logo.jpg`.
- **Taglines in use:** "Justice. Representation. Leadership." and "Empowering the next generation of Muslim lawyers and policymakers."
- **Voice:** earnest, civic and aspirational ("Your seat at the table starts here"), and the site addresses students directly.

## Evidence on Hand

- **Event photos** in `images/`: general meeting, large lecture, movie nights, "Moektails and Mock Trials" networking events, chapter members, and an about banner.
- **Chapter facts:** the six chapters with their cities and Instagram handles. Chapter emails are known for UCI and UCSD only.
- **Past speakers (confirmed by the user, okay to name):**
  - Farah Khan, former Mayor of Irvine
  - Assistant Dean of Admissions, UC Irvine School of Law (list by title only, no name)
  - Haaris M. Syed, Commissioner, Los Angeles County Superior Court
  - Siraj Bajwa, JD candidate, UC Irvine School of Law
- **Signature programs (recurring):** Mocktails & Mock Trials (spelled "Mocktails"; the old site's "Moektails" is a typo), speaker panels, policy workshops, and community nights (movie nights, general meetings, socials). Per-program details beyond the event photos are unconfirmed.
- **Mentorship has not launched.** The site may present it only as "coming soon" with an interest list for attorneys and students. Never present mentor matches, a running program or open applications as current.
- **Not available:** placement outcomes, partner organizations, testimonials, active mentors, and statistics beyond chapter count. Future work must not invent any of these.

## Product Principles

1. **Every audience gets a clear next step.** Students, founders and mentors each need an obvious path to act, and none of them should dominate the others.
2. **Claims stay within the evidence.** Show real events, photos and named people. Never invent outcomes, partners or numbers.
3. **One network, many chapters.** Present a national identity while respecting each chapter's independence.
4. **Keep it maintainable by one person.** Use plain static files, free services and no build tooling.
5. **Make private operations trustworthy.** Portal data, especially finances, is protected by server-side rules, not by obscurity.
