# Pylse PC Optimizer - STAGING update feed

**Not for use. Do not download anything here to run on your computer.**

This repository is the staging feed for the Pylse PC Optimizer's automatic updater. It holds test
releases and a `latest.json` that only special **staging builds** read. Those builds are compiled
with `-p:PylseStaging=true`, say "STAGING BUILD - NOT FOR RELEASE" in their title, and are used only
to prove the update path end to end before a release reaches the real feed:
- download;
- signature and checksum verification;
- replacement, restart and health check;
- refusal and rollback.

- **Normal copies of Pylse never read this feed.** Their feed address is compiled in and points at
  [`esh-dev-bartosz/pylse-optimizer-releases`](https://github.com/esh-dev-bartosz/pylse-optimizer-releases).
- **Some manifests here are deliberately broken.** They are unsigned, altered, or signed by an
  untrusted key, and some assets are deliberately damaged or deliberately fail to start. They exist
  to prove that Pylse refuses them.
- **Staging releases are signed with short-lived staging keys.** No released copy of Pylse trusts
  those keys.
- **The executables contain no source code, game configuration, credentials or user history.**

The real Pylse download is on [pylsetech.com](https://pylsetech.com).
