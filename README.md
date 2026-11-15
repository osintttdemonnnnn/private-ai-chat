# Afterglow — guest edition

No-login AI social website with character discovery, custom adult characters, personal feed, comments and character DMs. index.html loads guest.js; the prior account app.js is retained but unused. Guest mode never queries Supabase. Existing account data remains under its existing owner-only database policies.

Guest data stays in page memory by default. Optional unencrypted localStorage saving is available in Settings. Anyone using the same browser profile can access saved guest data. No account isolation or cross-device synchronization. Turning saving off removes the saved guest world. Reset clears app data, not backups or forensic records. The adult entry screen is self-attestation, not verified age assurance.

Text uses browser-side WebLLM and a local Llama model, downloaded on first generation or through Settings. Requires compatible WebGPU browser/hardware, memory and bandwidth. No paid inference fallback. Model refusals may occur. Image/video generation is not connected. Portraits are abstract CSS illustrations. Third-party CDN/fonts/model downloads receive network metadata and are trust dependencies.

No-login edition requires browser and model-loading tests after deployment. It is not a guarantee of runtime compatibility, unlimited free hosting, or complete privacy from device users or administrators.
