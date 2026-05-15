# Raw Sources

#system

> **Purpose:** Immutable archive of raw interview transcripts, meeting recordings, and source documents. Claude Code reads from this folder but NEVER modifies files in it.
> **Convention:** Files are named by date and source: `YYYY-MM-DD — Source Description.md`

---

## What goes here

- Raw interview transcripts (copy-pasted from transcription tools, .docx extracts, or chat)
- Raw standup/meeting transcripts
- Raw podcast transcripts or article text (for Market Intelligence)
- Any source document before it has been processed into a structured vault note

## What does NOT go here

- Structured interview notes (those go in 02-Research/)
- Strategy documents (those go in 01-Strategy/)
- Anything that has been edited, synthesised, or reformatted

## Workflow

1. Drop the raw transcript here
2. Tell Claude Code: "Process the raw file at 00-Raw/[filename]"
3. Claude Code reads it, creates the structured note in the appropriate folder, updates Patterns, Open Questions, and Home.md
4. The raw file stays here permanently as the source of truth
