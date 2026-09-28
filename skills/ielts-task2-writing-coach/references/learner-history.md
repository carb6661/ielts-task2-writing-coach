# Learner history format

Use this only after the learner has opted in to local progress tracking. Keep the JSON machine-readable and the Markdown summary short enough to review before a new writing session.

## `learner-history.json`

```json
{
  "learner": { "preferred_target_band": 7.0, "spelling_convention": "British English" },
  "essays": [
    {
      "date": "YYYY-MM-DD",
      "prompt_summary": "short neutral summary",
      "question_type": "opinion",
      "target_band": 7.0,
      "estimated_bands": { "overall": "6.5-7.0", "TR": "7.0", "CC": "6.5", "LR": "6.5", "GRA": "6.5" },
      "evidence": ["brief evidence-based observation"],
      "next_practice": "one concrete practice task"
    }
  ],
  "recurring_patterns": [
    {
      "category": "grammar|lexis|cohesion|task_response|argument",
      "pattern": "specific observable issue",
      "examples": ["short learner excerpt"],
      "occurrences": 1,
      "last_seen": "YYYY-MM-DD",
      "status": "active|improving|resolved"
    }
  ],
  "next_focus": "one highest-leverage skill"
}
```

Create the initial file with an empty `essays` and `recurring_patterns` list. Add a recurring pattern only after it appears in at least two separate essays, or label it as a one-off observation in the relevant essay instead.

## `learner-history.md`

Include:

1. current target band and latest estimated profile;
2. progress observations supported by two or more entries;
3. active recurring patterns with a short correction rule;
4. the next one or two practice priorities.

Do not copy full essays into the summary. When a learner asks to remove their history, delete only the explicitly identified history files after confirming their paths.
