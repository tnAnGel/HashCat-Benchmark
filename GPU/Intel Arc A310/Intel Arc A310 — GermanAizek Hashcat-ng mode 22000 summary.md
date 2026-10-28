# Intel Arc A310 — Hashcat-ng mode 22000 (summary-only)

- **Device attribution:** the source table names `Intel Arc A310` exactly.
- **Reported result:** mode 22000 (WPA-PBKDF2-PMKID+EAPOL), `157126 H/s`.
- **Evidence type:** one published scalar in a GPU comparison table. The source does not include the run's raw stdout, host, driver, command line, or benchmark date; this is not a reproducible raw capture.
- **Non-standard implementation:** the publisher explicitly identifies the table as a proprietary Hashcat-ng fork, not the FOSS/upstream Hashcat build. Do not compare or merge this score with upstream `hashcat -b` results.
- **Source:** [GermanAizek public Gist — Hashcat-ng mode 22000 GPU rating](https://gist.github.com/GermanAizek/f968d0bb213b2b7c8d9b35bbc4d031e4).

| Hash mode | Algorithm | Published speed | Status |
|---:|---|---:|---|
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 157126 H/s | Summary-only; proprietary fork; no raw run metadata |
