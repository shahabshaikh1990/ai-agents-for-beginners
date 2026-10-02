---
name: migrate-notebook-to-dotnet
description: Use when asked to convert a Jupyter notebook into Markdown plus a .NET single-file .cs sample.
---

Outcome: for the notebook in the request, a reader can follow the lesson without Jupyter.
- `<name>.md` beside the notebook: its narrative and code in original order, plain Markdown, one H1.
- If it contains C#, also `<name>.cs`, a runnable .NET single-file app (https://devblogs.microsoft.com/dotnet/announcing-dotnet-run-app/) holding the C# cells in order. The Markdown links to it instead of inlining the C#. Other languages stay inline.

Hard boundaries
- Never invent, change or execute code.
- No outputs, execution counts, metadata, empty cells or notebook JSON in the result.
- Leave the source notebook in place and say it is now redundant.
- No cells: stop and report. Create nothing.

Good looks like
- Correct language tag on every fence, no runs of blank lines.
- `.cs` starts with `#!/usr/bin/dotnet run`, then one `#:package Name@Version` per NuGet dependency, and is executable.
- Together `.md` and `.cs` contain every code cell, nothing lost or reordered.
