# Verification performed

The six supplied HTML files were SHA-256 checked against the recovered expected
hashes before copying. Each snapshot was copied without newline, encoding, source
or filename changes. The per-state manifests record file sizes and hashes.
Application code was inspected for loading, rendering, editing, persistence and
export behavior. Full MIT dependency notice accompanies every state.

This restoration does not claim browser interaction tests, automated behavioral
tests, successful Markdown round-trip tests, or fixes to original defects. The
independent prior source review reported no secrets/private payloads in these six
HTML sources; it also identified unsanitized innerHTML and plaintext local drafts.
That report is not a guarantee about documents a user may subsequently open.
