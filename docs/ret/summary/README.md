# summary/

Human-readable Chinese-language summaries of RET (After Action Record) documents.

## Rules

- **Language**: Chinese (中文)
- **Tone**: Storytelling (讲故事), may be humorous
- **Length**: 5–15 sentences
- **Naming**: 1:1 mapping with parent document (same filename)
- **Goal**: A reader who reads only the summary can say: "我知道这个文件在讲什么了。"

## Content requirements

- What decision was being implemented
- What actually happened vs. what was planned
- What was learned
- One sentence on what would break if this lesson were ignored

## What summaries are NOT

- Not translations of the full document
- Not technical specifications
- Not approval-gated (anyone can write or update them)

## Example

Parent: `docs/ret/RET-0008-0002-0001-symlink-approach-required-three-iterations.md`
Summary: `docs/ret/summary/RET-0008-0002-0001-symlink-approach-required-three-iterations.md`
