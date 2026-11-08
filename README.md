# tallymark-site

Public landing page for the **Tallymark market test** — a waitlist page for a
possible public version of Tallymark, a privacy-first money tracker for iPhone
(one-time purchase; optional bank sync via the user's own SimpleFIN Bridge
subscription; no developer server, data stored only on the user's device).

- Live at: https://sourweasel1.github.io/tallymark-site/
- `index.html` is a single self-contained file: no external CSS, JS, fonts, or
  tracking. Its only external call is the waitlist form POST.
- The waitlist form posts to Buttondown's embed-subscribe endpoint. The form
  action contains a placeholder username (`__BUTTONDOWN_USERNAME__`) that must
  be replaced with the real Buttondown account username before signups work;
  survey answers are sent as Buttondown subscriber metadata
  (`metadata__current_app`, `metadata__would_pay`, `metadata__setup_dealbreaker`).
