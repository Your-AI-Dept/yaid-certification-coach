# YAID Certification Coach

Choose a Claude certification, practise the concepts, and turn your results into a study plan. YAID Certification Coach supports Architect Foundations (CCAR-F), Developer Foundations (CCDV-F), Associate Foundations (CCAO-F), and Architect Professional (CCAR-P).

The coach provides a 15-question diagnostic, short domain drills with explanations, timed mocks, domain feedback, and practical ways to combine a credential with evidence clients can verify. The hosted YAID bank contains 383 practice questions. Independent preparation by Your AI Department; official certification is awarded by Anthropic.

![YAID mark](./assets/icon.svg)

## Start practising

Ask “Which Claude certification fits my AI consulting work?” or “Give me a CCDV-F diagnostic and a study plan.” Select your own answers. The coach explains study answers immediately and withholds diagnostic and mock explanations until completion. Scores are practice accuracy, not official exam scores or a guarantee of passing.

In Claude Code, load this folder with `claude --plugin-dir ./claude-plugin`, adjusting the path to your checkout. Then use `/yaid-certification-coach:certification-coach` or `/yaid-certification-coach:diagnostic ccdv-f`. To install from YAID’s repository, add the marketplace and install:

```text
/plugin marketplace add Your-AI-Dept/yaid-certification-coach
/plugin install yaid-certification-coach@yaid-certification
```

In Claude chat or Cowork, connect the hosted service through Customize → Connectors → Add custom connector, using `https://yaid-certification-coach.vercel.app/mcp` and no sign-in. This private test connection is separate from a directory installation. The plugin has not yet been approved or published in Anthropic’s directory.

Claude hosts that render MCP Apps can display the interactive practice card. Claude Code uses the text questions and tool responses. Actual rendering varies by host. The coach never takes an official exam or registers you for one.

## Requirements and permissions

An internet connection and a Claude client supporting remote HTTP MCP are required. No YAID membership, API key, local package installation, hooks or access to your project files is needed. The eight declared tools read YAID’s catalog, create and update anonymous practice attempts, retrieve results, explain access, and help plan evidence of consulting ability. Ending an attempt is final and unanswered questions count as incorrect.

## Privacy

The declared YAID endpoint receives exam choices, question IDs, selected answer IDs, assistance flags and session IDs. It stores practice attempts and timestamps in YAID’s Supabase database, with hosting by Vercel. Sessions expire after seven days; daily cleanup normally removes expired records within another 24 hours. The plugin does not request your name, email, full conversation, files or official exam credentials. A session ID grants access to its attempt, so keep it private.

Claude receives tool results and processes your conversation under Anthropic’s own policies. YAID’s application has no advertising, session replay or marketing tracking. Provider operational logs and backups have separate retention schedules. Read the [coach privacy notice](https://yaid-certification-coach.vercel.app/privacy) and [YAID privacy policy](https://youraidept.com/privacy-policy).

## Help and access

Ask the coach how certification access works. It will consider existing employer affiliation first and explain YAID’s route for independent practitioners, subject to acceptance and current eligibility. Practice does not purchase membership or guarantee exam access, certification, work or income.

For support or to report a question error, email contact@youraidept.com. Include the track and question ID, without official exam material. [YAID exam guides and practice](https://youraidept.com/network/claude-certification-practice-exam) · [Support](https://youraidept.com/faq) · [Terms](https://youraidept.com/terms-of-service).
