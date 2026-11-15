# Afterglow

Original AI social app with character discovery, personal feed, comments, custom adult characters, and character DMs. Not affiliated with Aspect or Candy AI. Abstract CSS portraits are illustrative placeholders, not generated photos.

## Accounts and privacy
Supabase email/password signup/login, session persistence, and user_worlds storage are integrated. Only the public publishable key is in browser code; no service-role key. The user_worlds table has forced RLS with owner-only SELECT/INSERT/UPDATE/DELETE policies. Signup may require email confirmation. Verify email delivery, templates, Auth Site URL and redirect allowlist for https://private-ai-chat-three.vercel.app in the Supabase dashboard before announcing registration works end-to-end. Default email service limits apply. Password recovery and account deletion are not implemented.

Worlds hold characters, posts, and chats in one JSON record with a 2 MB cap; concurrent updates are last-write-wins. Existing anonymous localStorage chats are not migrated. Sessions persist in browser storage; users should sign out on shared devices. Account-private is not end-to-end encrypted; administrators and relevant infrastructure retain their access. Third-party SDK/CDN/fonts are trust and metadata dependencies. No paid services enabled by this code.

## AI and media
Text inference uses WebLLM 0.2.79 and Llama-3.2-1B-Instruct-q4f16_1-MLC on visitors' devices. Compatible WebGPU hardware/browser, memory, and bandwidth are required. Model availability and browser runtime need testing. Model output is not guaranteed uncensored. Image/video generation is explicitly unavailable, with no paid fallback.

## Verification status
Supabase migration applied successfully and security advisor returned no warnings before this commit. Full two-user isolation tests, browser tests, model-load tests, email-confirmation flow, and mobile tests have not been completed. Database policies alone do not constitute a full security audit. Configure Auth redirect URLs and production email delivery as appropriate. Signup age declaration and adult character age validation are not verified age assurance. Review adult-content hosting and legal requirements before public operation.
