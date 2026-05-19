# ideaREG

**An open registry of ideas.**

## What this is

ideaREG is a public registry for ideas. Anyone can register an idea by adding a file to this repository. Each registration is timestamped, attributed (optionally), and cryptographically chained to the previous registrations through Git's commit history.

The purpose is to create a verifiable public record of who registered which ideas and when. The records can be used as prior-art evidence, as personal documentation, as contributions to a growing commons of openly-shared ideas, or as anything else the registrants choose.

## Why this exists

Ideas have always been hard to attribute reliably. The people who first have an idea are often not the people who can patent it, market it, or turn it into something commercial. Ideas drift around in conversations, notebooks, and partial implementations until someone with the resources to claim them does so — sometimes the original thinker, often not.

ideaREG is a small attempt to give ideas a public home where the timestamp of their first registration is verifiable, the attribution is preserved, and the underlying content is openly available for anyone to read and build on.

The longer-term hope is that registries like this one, accumulated across many contributors over time, can contribute to making patents meaningless by establishing public prior art at sufficient scale. This is an ambitious goal that ideaREG alone will not achieve. Contributing to the direction is what is in the actor's power to make.

## How to register an idea

The simplest path:

1. **Fork this repository** to your own GitHub account.
2. **Copy `TEMPLATE.md`** to a new file in the `ideas/` directory. Name the file something descriptive, such as `ideas/your-idea-name.md`.
3. **Fill in the template** with your name, the registration date, the idea origin date, the idea content, and any remarks.
4. **Submit a pull request** back to this repository.

The pull request will be reviewed and merged. Once merged, your idea is registered with the timestamp of the merge commit, attributed to you, and preserved in the repository's history.

If you have an Identor number assigned in the broader Identor system, you can include it in the registration. If you do not have an Identor number, leave the field blank. Identor numbers are not required for registration.

## Submission paths

Three submission paths are supported.

**Pull request from a fork.** The standard path, described above. Suitable for most contributors.

**Direct commit for trusted Identors.** Contributors who have established Identor numbers and trust with the maintainer can be granted direct write access to commit ideas without going through the pull request flow. Contact the maintainer to request direct access.

**Hash-only submission for secret ideas.** If you want to register an idea without revealing its contents, submit only the SHA-512 hash of the idea text along with the registration metadata. The hash establishes that the idea existed at the registration date. You can later disclose the original content and prove (by hashing the disclosed content and matching it against the registered hash) that the idea was yours as of the registration date.

For hash-only submissions, use the `HASH_TEMPLATE.md` file instead of the full template.

## License

All registrations in this repository are released under the **MIT License** unless otherwise specified by the registrant.

The MIT license applies to the registration documents themselves. The ideas described in the registrations are publicly disclosed by the act of registration and enter the public commons accordingly.

If you want to register an idea under a different license, specify it in the registration's License section. Common alternatives include CC BY 4.0 (attribution required, broader use rights), CC0 (public domain dedication), and Apache 2.0 (similar to MIT with explicit patent grant).

## Verification

Each registration's authenticity is verified by Git's commit history. Every commit contains the cryptographic hash of the previous commit, making the entire history tamper-evident. GitHub's commit timestamps are server-recorded and difficult to backdate.

To verify a registration's date, examine the commit history for the file in question. The earliest commit that contains the registration is the canonical registration date.

To verify a hash-only submission, the registrant must disclose the original idea content. Hashing the disclosed content with SHA-512 should produce the same hash that was originally registered. If the hashes match, the registration is authentic.

## The Identor system

Some registrations carry **Identor numbers**, which are part of a broader system used in the Antti Bible to recognise contributors whose ideas have meaningfully shaped the author's thinking. Identor numbers are assigned by the maintainer and are not awarded automatically with registration. Registrants without Identor numbers are equally welcome.

The Identor system is documented in the Antti Bible's foreword and in entries throughout the broader project. ideaREG is one operational expression of the system but does not require participation in the broader Bible.

## What this is not

ideaREG is not a patent system. Registration here does not grant any legal rights to the registrant beyond what they would have anyway under copyright and trade-secret law.

ideaREG is not a guarantee of priority. Other people may have had the same idea earlier, in private notebooks or in unpublished conversations. Registration here establishes that you publicly disclosed the idea on the registration date; it does not establish that you were the first person to think of it.

ideaREG is not a commercial service. It is a public open-source project maintained by Antti Lukats. There are no fees, no membership tiers, no premium features.

## Contact

The maintainer of ideaREG is **Antti Lukats** (Identor #1).

Issues, questions, and suggestions can be filed in this repository's GitHub Issues. Pull requests are welcome.

---

*ideaREG is part of the broader Antti Bible project.*
*Repository: github.com/micro-FPGA/ideaREG*
*First registration: "Generation AI" by Identor #1, 6 May year 7 AG (2026).*
