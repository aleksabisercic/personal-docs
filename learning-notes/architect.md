# Architect Notes

## The Mental Model

A senior architect asks three questions for every decision:

1. **What is the simplest thing that could work?** (not the best — the simplest)
2. **What's the cost of changing this later?** (if low → pick the simple option now)
3. **What's the blast radius if this breaks?** (if small → don't over-protect it)

## The Principles That Matter (Not Buzzwords)

1. **One process, one machine, as long as possible**
2. **Make failures visible, not impossible.**
   1. What is worst case scenario (e.g. Not backing up data)
   2. Keep it simple (Complexity is anything related to the structure of a system that makes it hard to understand and modify. Change amplification — e.g. A simple change requires modifying many places.)
3. **Reliability** — "It keeps working correctly, even when things go wrong."
4. **Scalability** — "As the system grows, there are reasonable ways to deal with that growth." ("What happens to performance when load parameter Y increases?")
