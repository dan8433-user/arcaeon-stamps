# arcaeon-stamps

Public record for Arcaeon file stamps.

Each stamp is one commit in this repository. A stamp records the SHA-256 fingerprint of a file and its size in bytes, and nothing else. The file itself never leaves the computer of the person who stamped it. No file names, no file contents, and no personal details are stored here.

## What a stamp shows

That a file with this exact fingerprint was on this public record no later than the date of its commit. The first stamp for a fingerprint is the one that counts. Stamping the same file again returns the original record and writes nothing new.

## What a stamp does not show

- Who made the file, who owns it, or who stamped it.
- That the contents of the file are true, original, or lawful.
- That the file did not exist earlier than the stamp.
- It is not a qualified electronic timestamp under eIDAS or any other statute, and it is not legal advice.

## Checking a stamp yourself

Compute the SHA-256 of the file on your own machine and look for that fingerprint in this repository. The commit history is public, and anyone can clone or mirror this repository at any time. A copy made today cannot be changed by Arcaeon afterwards, so if a record here were changed or replaced after the fact, the history and any earlier copy would show it. A commit date on its own is a statement by whoever wrote the commit; what gives it weight is that the record is public and copied from the moment it is written. You do not need to contact Arcaeon or trust Arcaeon's servers to make this check.

## Layout

`stamps/<first two hex characters>/<full fingerprint>.json` holds one stamp. `stamps/_meta/` holds the service's own daily counters and no customer data.

## Operator

Arcaeon. This repository is written to only by the Arcaeon stamp service.
