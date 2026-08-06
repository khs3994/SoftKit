<p align="center">
  <img src="assets/banner.png" alt="SoftKit" width="480">
</p>

# SoftKit

A toolkit for automating the soft side of software development — planning, docs, and communication.

Writing code is only part of the job. SoftKit is a Claude plugin for everything around it: reviewing specs before work starts, sanity-checking estimates, planning sprints, and turning messy context into documents other people can actually read.

Its counterpart, [HardKit](https://github.com/khs3994/HardKit), handles the code itself.

## What's inside

**Communication**

- **`surface` skill** — scans the current session for what's worth sharing and surfaces the ambiguous spots that still need someone's answer, then drafts a per-recipient message you can paste into Slack. Drafts only; it never sends.
- **`communicator` agent** — a general-purpose communication specialist that turns dev context into a clear, appropriately-toned message for a specific audience. Reusable on its own, and the drafting engine behind `surface`.

More kits (specs, estimates, planning, docs) to follow.

## License

MIT
