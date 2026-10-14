# Sahmaoi

Robotics engineer, software builder, turtle enthusiast. I run [VTEC](https://vtec-jo.com) (Venture Tech Engineering Consultancy LLC) and build products for small businesses, in English and Arabic.

My engineering philosophy is borrowed from turtles: move steadily, carry your armour with you, and outlive the people who rushed.

## Building

- **OrbitBook** ([orbit-book.com](https://orbit-book.com)): appointment booking for service businesses. Customers book from a public page with no account; owners run branches, staff, hours and bookings from one dashboard. Full Arabic with right-to-left layout. Phase 2 (branches, roles, an admin console) ships soon.
- **Delta-V**: VTEC's project cost tracker. Plans a project's budget up front and tracks what it actually spends, the way a mission plans its delta-v. It retired a spreadsheet that had seen things. Next.js, Drizzle and Postgres, self-hosted in Docker.

## Agent orchestration

I don't prompt one AI. I run a team of them, and none of them gets to merge without passing review.

- **19 specialist agents**: implementers, a code reviewer, a security auditor, a scale-breaker whose whole job is to attack every change, a threat modeller, release and supply-chain checks, and one reviewer that exists purely to reject anything that sounds like a robot wrote it.
- **The shell**: git hooks that refuse a commit the scale-breaker hasn't cleared, and scan every commit for secrets. Nobody gets past them, me included.
- **A shared second brain**: every solved problem gets written down, and every agent reads it before starting, so the same mistake never costs twice.
- **Claude Code mods**: a live task board, a signal that pings me when an agent needs a human, and a cap on how many agents run at once, because ten agents in parallel is just chaos with better PR.

## How I build

Control systems taught me to design for failure first: a retry that never double-books, data that gets deleted when the policy says it does, an alert that fires once instead of fifty times.

## Stack

Next.js · TypeScript · React · Supabase (Postgres, row-level security, Edge Functions) · Drizzle · Cloudflare Workers · Docker · Python · Claude Code

## Off the clock

- Turtles. Watching them, reading about them, defending them in arguments. A 100-year-old tortoise has better uptime than most production systems.
- Fuecoco is the correct starter. This is not up for discussion.
