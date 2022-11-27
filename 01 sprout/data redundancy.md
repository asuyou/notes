# data redundancy
---
Topics: #redundancy
Created: 2022-07-20 21:58:12

---

We can use RAID

## RAID-0

Provides data striping across multiple disks to increase performance but without fault tolerance.

## RAID-1

Mirroring to a 2nd drive

Fault-resistant / Fault-tolerant

## RAID-5

Requires at least 3 disks. It stripes data across disks and write parity data across these drives too

Fault-resistant / Fault-tolerant

## RAID-6

Modified version of [[#RAID-5]] but uses 2 stripes of parity data instead of 1

Fault-tolerant

## RAID-10

Creates a striped RAIN of 2 mirrored RAIDs

Combines [[#RAID-1]] and [[#RAID-0]]

Requires 4 drives

Disaster-tolerant

# References
