# Afterglow

Original Aspect-inspired AI social website. Not affiliated with Aspect and does not copy its branding or assets. Features: personal AI feed, comments, generated character posts, adult character creation, separate character DMs, optional device-local persistence, and deletion controls. No image generation, autonomous background activity, user accounts, shared database, or cross-device sync.

## Status
Initial implementation, not browser-tested or deployed by this commit. Uses WebLLM 0.2.79 from esm.run and Llama-3.2-1B-Instruct-q4f16_1-MLC. Verify dependency availability, model compatibility, and runtime behavior before launch. The general-purpose model may refuse adult requests. No promise of completely uncensored output.

## Hosting
Static files can be served over HTTPS. Repository creation and code commits do not publish a site. Choose a host whose current acceptable-use policy permits your intended content. Review GitHub adult-content and Pages restrictions before considering Pages for an adult-oriented site. Hosting, CDN, and model distribution have limits and terms; unlimited free service is not guaranteed. No paid inference API is included; visitors supply compute, memory, bandwidth, and electricity.

## Privacy
Messages, feed posts, and characters stay in page memory unless local saving is enabled. This implementation intentionally sends no chat content to an inference server. Saved worlds use unencrypted localStorage, with no account separation within a shared browser profile. Other sites on the same origin, extensions, third-party dependencies, or a compromised device can affect privacy. Hosting/CDN/model hosts receive network metadata. Public repository source does not contain visitor conversations. Deletion clears app storage, not backups or forensic traces. Audit and self-host dependencies for stronger assurance.

## Adult content and safety
The entry screen is an 18+ self-attestation, not identity verification or a guarantee of legal compliance. Characters must have adult ages. The system prompt prohibits sexual content involving minors and non-consensual sexual activity; prompts are not reliable moderation enforcement. Public adult services may require additional jurisdiction-specific safeguards. No image uploads or explicit media assets are included.
