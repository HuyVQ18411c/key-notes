# MIT6824 Distributed Systems
Course: [Youtube](https://www.youtube.com/playlist?list=PLrw6a1wE39_tb2fErI4-WkMbsvGQk9_UB)

# Notes

### Why do we need Distributed systems:
- Hardwares get cheaper => Gain more benefits while use them concurrently
- Prevent single point failure (fault tolerance)
- Security, compliance: isolate all data/logic

### MapReduce
- Originally produced by Google
- Assume there are chunks of data (ex: multiple files), runs `Map` function on each chunk and produce a key-value output (intermediate output) -> collect all same keys into a collection -> pass each collection to a `Reduce` function (kinda similar to array.reduce of JavaScript). Each of Map and Reduce is a job/task.