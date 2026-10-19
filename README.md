NJ Motors — used-car dealership website

> The client's code is private at their request. This is a write-up of what I built and how.

A full website for a used-car dealership. The owner manages stock, enquiries and page content through an admin panel, so day-to-day changes need no developer.

Status: in development, launching soon.

Stack
Next.js · TypeScript · Payload CMS · Neon (PostgreSQL) · Vercel · Vercel Blob · Resend · GSAP

What I built
- Payload CMS collections for vehicles, enquiries and site content, editable without code
- Vehicle listing and detail pages driven by the CMS, with image storage on Vercel Blob
- Enquiry form sending email through Resend, with domain verification
- A scroll-animation layer on top of the CMS-driven pages, kept separate from the data layer
- Pre-launch audit: fixed a database schema issue in Neon, set up environment config and the Vercel deploy pipeline

What was hard
- [one honest sentence about the Neon schema blocker]
- Keeping the animation layer separate so backend changes don't break the frontend
- Writing site copy to the client's exact wording rather than my own
