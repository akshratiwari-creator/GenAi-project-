# Meeting Notes

A local Python 3.10+ app. It has no packages to install.

1. Open PowerShell in this folder.
2. Set your OpenAI API key for this PowerShell session. To enter it without saving it in command history, run:

   ```powershell
   $env:OPENAI_API_KEY = [System.Net.NetworkCredential]::new('', (Read-Host 'OpenAI API key' -AsSecureString)).Password
   ```

3. Run `py app.py` and open http://127.0.0.1:8765.
4. Paste a transcript or open a UTF-8 text file. Select **Generate notes**. You can download the complete record or copy the follow-up email.

**Try sample** shows a prepared example without an API key. For your own transcripts,
the app sends text to OpenAI using the configured account. It defaults to
`gpt-4o-mini`. Set `OPENAI_MODEL` before launching to use another model that
supports Chat Completions JSON mode. Stop the server with Ctrl+C.
