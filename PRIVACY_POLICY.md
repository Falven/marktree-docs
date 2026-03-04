MarkTree Privacy Policy

⸻

1. Introduction

Thank you for using MarkTree ("the Extension"). This Privacy Policy explains what data the Extension accesses, how that data is used, and the limited circumstances in which data leaves your device. By installing or using the Extension, you agree to the practices described below.

⸻

2. Scope

This policy covers the MarkTree free feature set and the optional MarkTree Pro license add-on published in the Visual Studio Marketplace. It applies only to data handled by the Extension.

⸻

3. Information we process

Category | What is accessed | Where it is processed | When it is transmitted off-device
Workspace content | File paths, file contents, directory structure, open tabs, selected text, diagnostics, Git diffs (via git CLI) | Entirely on your local machine (main VS Code process and a background worker thread) | Never. Content is copied only to your local clipboard; the Extension does not send it anywhere.
Clipboard data | Markdown produced from the items above | Local clipboard API | Never (unless you paste it into another app or website).
License data (Pro users only) | License key you enter; time-limited token returned by server | The key is stored in VS Code Secret Storage. The license key is sent once per validation over HTTPS to our licensing endpoint. No workspace content is included. | License validation request only.
Settings and preferences | Feature toggles such as ignore binary files, notification settings, and custom ignore lists | Saved in your local `.vscode/settings.json` or global VS Code settings | Never.
Model metadata (token counter only) | Public model metadata from OpenRouter used for token-counter model selection | Fetched at runtime, then cached in VS Code extension state | Sent only when fetching model metadata from OpenRouter.

The Extension does not collect analytics, telemetry, advertising identifiers, or location data.

⸻

4. How we use the information

Purpose | Legal basis (GDPR)
Execute the commands you invoke (for example copy files, build Markdown, run git show) | Legitimate interest in providing requested functionality
Validate and enforce MarkTree Pro licenses | Contract performance (End-User License Agreement)
Show error logs in the Output panel | Legitimate interest in debugging and improving the Extension

⸻

5. Data storage and retention

- Workspace content exists only in process memory and your clipboard.
- License key and token (Pro) remain in Secret Storage until you clear the key, uninstall the Extension, or validation state changes.
- Token-counter model metadata is cached locally in extension state for performance and refreshed periodically.

⸻

6. Sharing and disclosure

We do not sell, rent, or share your code or personal data. We disclose information only if required by law.

⸻

7. Security

- Local secrets are stored using VS Code encrypted storage APIs.
- License validation and model-metadata requests use TLS 1.2+.
- Worker threads run in a separate Node.js context to isolate file-system-heavy operations.

No method of electronic transmission or storage is perfectly secure. Use the Extension at your own risk and avoid copying confidential material if that violates your organization’s policies.

⸻

8. Third-party components

The Extension uses open-source libraries (for example `clipboardy`, `p-retry`, `binary-extensions`) that run locally. License validation is hosted on Azure. Token-counter model metadata is fetched from OpenRouter.

⸻

9. Your rights

If you reside in a jurisdiction with data-protection laws (for example GDPR or CCPA), you may have rights to access, correct, or delete personal data we hold about you. Because MarkTree stores only license-related data and local settings/caches, you can exercise these rights by clearing your license key and local extension data or by contacting us (see § 12).

⸻

10. Children’s privacy

MarkTree is not directed to children under 13. We do not knowingly collect personal data from children.

⸻

11. Changes to this policy

We may update this Privacy Policy to reflect changes in functionality or legal requirements. Material changes will be announced in release notes and will not retroactively reduce your privacy rights without explicit consent.

⸻

12. Contact

For questions or concerns about this policy, email privacy @ marktree.dev.

⸻

Last updated: 4 March 2026
