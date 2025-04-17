MarkTree Privacy Policy

⸻

1. Introduction

Thank you for using MarkTree (“the Extension”). This Privacy Policy explains what data the Extension accesses, how that data is used, and the limited circumstances in which data leaves your device. By installing or using the Extension you agree to the practices described below.

⸻

2. Scope

This policy covers the MarkTree free feature‑set and the optional MarkTree Pro licence add‑on published in the Visual Studio Marketplace. It applies only to data handled by the Extension; it does not cover any third‑party services you may interact with (e.g. GitHub, Azure, LLM providers) after the Extension copies content to your clipboard.

⸻

3. Information we process

Category What is accessed Where it is processed When it is transmitted off‑device
Workspace content File paths, file contents, directory structure, open tabs, selected text, diagnostics, Git diffs (via git CLI) Entirely on your local machine (main VS Code process and a background worker thread) Never. Content is copied only to your local clipboard; the Extension does not send it anywhere.
Clipboard data Markdown produced from the items above Local clipboard API Never (unless you paste it into another app or website).
Licence data (Pro users only) Licence key you enter; time‑limited token returned by server The key is stored in VS Code’s encrypted Secret Store. The licence key is sent once per validation over HTTPS to our licensing endpoint. No workspace content or personal identifiers are included.
Settings & preferences Feature toggles such as “ignore binary files”, “show notifications”, custom ignore lists Saved in your local .vscode/settings.json or global VS Code settings Never

The Extension does not collect analytics, telemetry, advertising identifiers, or location data.

⸻

4. How we use the information

Purpose Legal basis (GDPR)
Execute the commands you invoke (e.g., copy files, build Markdown, run git show) Legitimate interest in providing requested functionality
Validate and enforce MarkTree Pro licences Contract performance (End‑User Licence Agreement)
Show error logs in the Output panel Legitimate interest in debugging and improving the Extension

⸻

5. Data storage & retention
• Workspace content exists only in process memory and your clipboard; it is never written to disk by the Extension.
• Licence key & token (Pro) remain in Secret Store until you:
• run “MarkTree: Clear Licence Key”, or
• uninstall the Extension, or
• the token expires and validation fails.

We do not maintain any server‑side logs that link a licence key to a user identity.

⸻

6. Sharing & disclosure

We do not sell, rent, or share your code or personal data. We will disclose information only if required by law.

⸻

7. Security
• Local secrets are stored with VS Code’s encrypted storage APIs.
• Licence validation requests are sent over TLS 1.2+.
• The Extension’s worker threads run in a separate Node.js context to isolate file‑system access.

Despite these measures, no method of electronic transmission or storage is perfectly secure. Use the Extension at your own risk and avoid copying confidential material if that violates your organisation’s policies.

⸻

8. Third‑party components

The Extension uses open‑source libraries (e.g. clipboardy, p-retry, binary-extensions) that run locally and do not transmit your data. Licence validation is securely hosted on Azure.

⸻

9. Your rights

If you reside in a jurisdiction with data‑protection laws (e.g., GDPR, CCPA), you may have rights to access, correct, or delete personal data we hold about you. Because MarkTree stores only licence‑related data, you can exercise these rights at any time by clearing the licence key within VS Code or by contacting us (see § 12).

⸻

10. Children’s privacy

MarkTree is not directed to children under 13. We do not knowingly collect personal data from children.

⸻

11. Changes to this policy

We may update this Privacy Policy to reflect changes in functionality or legal requirements. Material changes will be announced in the release notes and will not retroactively reduce your privacy rights without explicit consent.

⸻

12. Contact

For questions or concerns about this policy, email privacy @ marktree.dev.

⸻

Last updated: 17 April 2025
