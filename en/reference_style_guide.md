# SCRF: Style Guide

The SCRF Community Writing Style Guide summarizes the standards and best practices authors should follow when contributing to Community Development resources.

## Writing Intent and Tone

SCRF materials should cater to readers who are unfamiliar with the SCRF system. Writers should also assume that their readers have tight schedules and short attention spans.

As such, Writers should focus on communicating concepts as clearly and succinctly as possible.

- Use simple language.
- Use short, concise sentences.
- Avoid unnecessary words.
- Remain open and objective.
- Provide examples when possible.
- Provide examples to help explain concepts, but avoid complicating them.
- Use math when necessary, but keep it simple.
- Link to basic terms if necessary.

## Writer Guidelines

### General Rules

- Run all drafts through [Grammarly](https://app.grammarly.com/) regularly, and before final submissions.
  - Grammarly will catch most spelling and grammatical errors.
  - Copy rendered text into Grammarly and address any mistakes it flags.
    - HackMD does not identify spelling and grammatical errors.
    - Grammarly will miss errors if it's given raw Markdown text.
    - Be careful of copy and pasting code from Grammarly to VScode, Grammarly may mess with formatting.

#### When migrating to a new document

- Leave a note in the old file.
- Provide a link to the latest version.
- Do not blindly accept Grammarly suggestions.
- Review edits to make sure they make sense.

#### Use

- [Oxford commas.](https://en.wikipedia.org/wiki/Serial_comma)
- [Pluralized, gender-neutral pronouns.](https://en.wikipedia.org/wiki/Singular_they)
  - Use "they/their" instead of "he/she/his/hers."
  - Examples: "When they..." or "If users choose to X, then their..."
- The % symbol. Do not spell out "percent."
  - Correct: 15%
  - Incorrect: 15 percent
- Double quotes `" "` for phrases, quotes, etc.
  - Do not use single `' '` quotes.

#### Avoid

- [First-person language.](https://en.wikipedia.org/wiki/Grammatical_person)
  - Examples: I, we, our, etc.
- [Second-person language](https://en.wikipedia.org/wiki/Grammatical_person) (unless it is appropriate for a guide or action page).
  - Examples: "You then..." or "Now you should..."
- Exclamation points.
- Footnotes.
- Parentheses for stating additional information.
  - Incorrect: Research Grants are larger-sized ($5,000 to $50,000) grants aimed at individuals or teams building projects.
  - Correct: Research Grants are generally larger-sized grants, ranging from $5,000 to $50,000, aimed at individuals or teams building projects.

### Abbreviations

- Use parentheses to define abbreviated terms the first time they appear in a given document.
  - Example: A Research Improvement Proposal (RIP) is a proposal framework to support new initiatives and to expand the scope of existing ones.
- Do not provide an abbreviation for a term that is only used once.

### Acronyms, Decades, and Cases

- Do not use apostrophes to pluralize acronyms or indicate decades. Add an "s" at the end.

#### Acronyms

- To make an acronym plural:
  - Correct: RIPs
  - Incorrect: RIP's

#### Decades

To indicate a decade:

- Correct: 1990s
- Incorrect: 1990's

#### Capitalize

- Names and proper nouns.
- Cities, countries, nationalities, and languages.
- Terms with definitions.

#### Title Case

- The [Title Case Converter](https://titlecaseconverter.com/) will keep titles consistent.
- Follow _The New York Times_ standard.
- Capitalize the first and last words, all nouns, pronouns, verbs, adverbs, and adjectives.
- Lowercase all articles, conjunctions, and prepositions.

### Currencies

The examples below use dollars, but the same rules apply to all global currencies.

- Use lowercase except when writing "US Dollar."
- Use figures and the "\$" sign in all except casual references, or amounts without a figure.
  - Standard: "The book costs $4."
  - Casual: "Please give me a dollar."
- For amounts under \$1 million, follow this format:
  - Correct: \$4, \$25, \$500, \$1,000, \$650,000.
- For amounts over \$1 million, use the word, not numerals.
  - Correct: "He is worth \$4 million."
  - Incorrect: "He is worth \$4,000,000."

### Cryptocurrencies

- When directly referring to the creation, destruction, or manipulation of a token (particularly as it relates to tooling):
  - Use the capitalized TLA version: DAI
  - Example: "Draw DAI against ETH from a Vault."
- Similarly, when referring to exchange pairs:
  - Use: ETH/DAI
- When referencing the token as a currency, in an instructional or conversational setting, or as a conceptual product of the Foundation or its systems:
  - Use: Dai
  - Example: "Dai is a price-stable asset that can be used as money."

### Numbers

- Spell out numbers below 10.
  - Examples: one, two, three, etc.
- Use numerals for numbers above 10, unless starting a sentence.
- For numbers with million, billion, or trillion, use figures in all except casual cases.
  - Standard: "The nation has 1 million citizens."
  - Casual: "I'd like to make a billion dollars."

### Lists

When bulleted and numbered lists contain complete sentences, capitalize the first word, and follow each with a period. If list items are phrases, no capitalization or punctuation is required.

- Use [parallel construction](https://en.wikipedia.org/wiki/Parallelism_%28grammar%29) for each item in a list.
- Start with the same [part of speech](https://en.wikipedia.org/wiki/Part_of_speech) for each item (in this case, a verb).
- Use the same verb [tense](https://en.wikipedia.org/wiki/Grammatical_tense#English) for each item.
- Use the same [voice](https://en.wikipedia.org/wiki/Voice_%28grammar%29) for each item.
- Use the same sentence type (statement, question, exclamation) for each item.
- List items that include definitions should look like this:
  - **Team:** Core team and Advisers are critical to SCRF's success.
  - **Community:** Sentiment analysis is invaluable.
- Use dashes rather than asterisks for unordered lists.
  - Correct: -
  - Incorrect: *
- Alphabetize lists of names unless there is a clear priority at work.
- Do not use ordered (numbered) lists unless order matters.
- Ordered list items should use the #1 repeated.
  - Markdown will automatically generate numbers.

Example:

```markdown
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b
```

### Links

- Use [relative links](https://docs.microsoft.com/en-us/contribute/how-to-write-links) when cross-referencing files from [repositories](https://github.com/smartcontractresearchforum/research_team) on SCRF's GitHub.
- Use [absolute links](([https://docs.microsoft.com/en-us/contribute/how-to-write-links](https://docs.microsoft.com/en-us/contribute/how-to-write-links))) and standard web URLs when referencing external resources.
- Create descriptive hyperlinks and avoid generic language.
  - Descriptive: Learn more at [Smart Contract Research Forum.](https://smartcontractresearch.org)
  - Generic: Learn more [here.](https://smartcontractresearch.org)
- Include a `.` inside the link for sentences that end with a link.

## Naming Conventions

All title of the docs should match the file names which should match the named links in other docs. Please do not use shorthand or new terms for existing documents. All document names should use 'snake case'.
