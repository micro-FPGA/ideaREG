# ideaREG Hash-Only Idea Registration

## Registrant

**Name:** FULL_NAME
**Identor #:** (leave blank if not assigned)
**Registration date:** YYYY-MM-DD
**Idea origin date or period:** YYYY-MM-DD or YYYY or "approximately YYYY-YYYY" or other recollection

## Hash

**Algorithm:** SHA-512
**Hash value:** (paste the 128-character hex string of your idea content here)

## Idea Title

(Optional: a short title or topic indicator that does not reveal the idea content. Examples: "Improvement to LDPC decoder architecture", "Method for reducing FPGA boot time", "Novel use of capacitor self-discharge for X". Leave blank if even the title would reveal too much.)

## Disclosure plan

(Optional: when and how you intend to disclose the full idea content. Examples: "Within 12 months", "Upon publication of related patent", "When commercial product launches", "Indefinitely private". Leave blank if you have no specific plan.)

## Remarks

(Optional: anything else worth recording that does not reveal the idea content.)

## License

This registration is released under the **OLL** unless otherwise specified.
The hash itself is freely shareable. The underlying idea remains private with the registrant until disclosed.

---

## How to verify this registration later

When the registrant discloses the original idea content, anyone can verify the registration's authenticity by:

1. Taking the original idea content (the exact text or file that was hashed at registration).
2. Computing its SHA-512 hash using any standard tool. On Linux or macOS: `sha512sum filename` or `shasum -a 512 filename`. On Windows PowerShell: `Get-FileHash -Algorithm SHA512 filename`.
3. Comparing the computed hash to the hash recorded in this registration.

If the hashes match exactly, the registration is authentic. The original idea content existed in its current form on the registration date.

If the hashes do not match, either the disclosed content is not the same as what was originally registered, or the registration is not authentic.

## Notes on hash-only registrations

The hash-only path is for ideas where the registrant wants to establish a verifiable timestamp of when the idea existed without disclosing the idea content publicly.

The hash establishes that *some specific content existed at the registration date*. It does not establish what the content was. A registrant who hashes "the secret of cold fusion is X" cannot later prove anything about cold fusion by pointing to the hash; they can only prove that the specific text "the secret of cold fusion is X" existed on the registration date.

For the hash to be useful as prior-art evidence, the original content must be preserved by the registrant in a form that can be reproduced exactly. Even small changes (different line endings, different character encoding, different whitespace) will produce a different hash. Common practice is to save the original idea content as a plain text file, in a known encoding (UTF-8 is standard), and to keep multiple backup copies.

Hash-only registrations cannot be modified. Once registered, the hash is immutable. If the registrant later decides to update the idea, they should submit a new registration with a new hash referencing the previous registration.

---

*This registration's authenticity is verified by the Git commit history of the ideaREG repository.*
*ideaREG: github.com/micro-FPGA/ideaREG*
