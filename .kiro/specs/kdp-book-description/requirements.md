# Requirements Document

## Introduction

This document specifies the requirements for creating KDP (Kindle Direct Publishing) retail copy for the novel *Seen and Still Loved* by D Allen Norris. The deliverable is a single Markdown file containing three purpose-built versions of the book description: an HTML-formatted Amazon listing description, a plain-text blurb, and back cover copy. All three versions serve a shared goal — to convert the right reader at the point of discovery — while honoring a set of authorial constraints about how the story's central secret is framed, how faith content is weighted, and how the book presents itself without relying on comparable titles.

The novel is a contemporary literary romance. The female lead, Maya Vasquez, carries a profound secret about her body that she has never disclosed to anyone she has been intimate with. Ethan Calloway, an exhibition designer and photographer, does not flinch. The story is about being fully seen and still loved. The title's promise — *seen completely, hidden from nothing, and still chosen* — is paid off at the wedding.

---

## Glossary

- **KDP Description**: The long-form product description displayed on a book's Amazon listing page, entered in HTML format, with a maximum length of 4,000 characters including HTML tags.
- **Plain-Text Blurb**: A version of the book description formatted without HTML markup, suitable for use in press kits, pitch materials, author website copy, and non-HTML retailer fields.
- **Back Cover Copy**: A tightly condensed version of the book description (approximately 150–200 words) formatted for physical or print-on-demand back cover placement, with a punchy closing line.
- **Maya Vasquez**: The female lead of the novel. An intersex woman whose specific medical condition is never named in any retail copy, per authorial constraint.
- **Ethan Calloway**: The male lead. Exhibition designer and film photographer. His acceptance of Maya's secret is the emotional fulcrum of the story.
- **The Managing Voice**: Maya's internal mechanism for controlling what she shows the world — a construct the narrative frames as exhausting, and which Ethan's presence begins to silence.
- **The Secret**: Maya's undisclosed physical reality. In all retail copy, this is described only as "a secret she has never shown anyone" or equivalent phrasing. The intersex identity is never named.
- **The Output File**: The Markdown file `kdp-description.md` to be saved in the `/Publish/` directory of the project workspace.

---

## Requirements

### Requirement 1: Three-Version Output Structure

**User Story:** As the author, I want a single file containing all three versions of the description, so that I can copy the relevant version for each publishing or promotional use case without searching across multiple files.

#### Acceptance Criteria

1. THE Output File SHALL contain three clearly labeled sections: an HTML-formatted KDP description, a plain-text blurb, and back cover copy.
2. THE Output File SHALL be saved at the path `/Users/norris/Documents/projects/writing/Authors/D Allen Norris/Seen and Still Loved/Publish/kdp-description.md`.
3. THE Output File SHALL use Markdown headings to separate each version so the document is navigable.

---

### Requirement 2: HTML KDP Description Formatting and Length

**User Story:** As the author, I want the Amazon description field populated with correctly formatted HTML that renders well on the Amazon listing page, so that the copy is visually compelling and passes KDP's formatting rules.

#### Acceptance Criteria

1. THE KDP Description SHALL be formatted using only HTML tags supported by Amazon KDP: `<h2>`, `<b>`, `<em>`, `<ul>`, `<li>`, `<br>`, and `<p>`.
2. THE KDP Description SHALL NOT exceed 4,000 characters in total length, including all HTML tags.
3. THE KDP Description SHALL open with a hook — a single bold line or short paragraph that stops a browsing reader — rather than with the author's name or the book's title.
4. THE KDP Description SHALL use structural breaks (paragraph tags or line breaks) to maintain readability; body text SHALL NOT be presented as a single unbroken block.
5. WHEN the KDP Description uses a closing line, THE KDP Description SHALL end with the thematic statement that encapsulates the title's promise: being seen completely and still chosen.

---

### Requirement 3: Plain-Text Blurb Formatting

**User Story:** As the author, I want a clean plain-text version of the description, so that I can paste it into press kits, pitch emails, and retailer fields that do not accept HTML.

#### Acceptance Criteria

1. THE Plain-Text Blurb SHALL contain no HTML markup of any kind.
2. THE Plain-Text Blurb SHALL be 250–400 words in length.
3. THE Plain-Text Blurb SHALL be self-contained — it SHALL convey the novel's premise, emotional stakes, and central promise without relying on the reader having seen any other version.

---

### Requirement 4: Back Cover Copy Formatting

**User Story:** As the author, I want a back cover copy version, so that I have purpose-built text for physical or print-on-demand editions that requires tighter word count and a punchy closing line.

#### Acceptance Criteria

1. THE Back Cover Copy SHALL be 150–200 words in length.
2. THE Back Cover Copy SHALL end with a single punchy closing line (one sentence, no more than 15 words) that delivers the emotional promise of the title.
3. THE Back Cover Copy SHALL be formatted in short, visually manageable paragraphs appropriate for back cover layout.

---

### Requirement 5: Maya's Secret — Implied, Not Named

**User Story:** As the author, I want Maya's intersex identity to remain implied in all retail copy, so that readers encounter her secret as she experiences it — as something deeply personal and unnameable — rather than as a medical label that may trigger incorrect assumptions or reduce the story to a single-issue narrative.

#### Acceptance Criteria

1. THE Output File SHALL NOT use the words "intersex," "chimerism," "chromosom*," "hermaphrodite," or any clinical or anatomical terminology referring to Maya's condition in any of the three versions.
2. WHEN all three versions refer to Maya's secret, THE descriptions SHALL use phrasing that conveys profound hiddenness without naming the nature of the secret — for example: "a secret she has never shown anyone," "something she has carried her entire adult life," or equivalent.
3. THE descriptions SHALL frame the secret as Maya's lived experience and emotional burden, not as a category or diagnosis.
4. THE descriptions SHALL convey that the secret involves physical vulnerability and intimacy — sufficient for a reader to understand the stakes of disclosure — without explicit anatomical description.

---

### Requirement 6: Faith Content — Light Touch Only

**User Story:** As the author, I want faith themes acknowledged with a single passing nod, so that readers for whom faith is meaningful feel the thread is present without positioning the novel as Christian fiction or inspirational romance.

#### Acceptance Criteria

1. WHEN faith content appears in any of the three versions, THE version SHALL reference faith with no more than one phrase or clause — not a dedicated sentence, and never a dedicated paragraph.
2. THE Output File SHALL NOT use phrases that signal Christian fiction genre marketing ("inspirational," "faith journey," "Christian romance," "God's plan") in any of the three versions.
3. THE Output File SHALL NOT include a scripture reference (e.g., "Psalm 139:14") in any of the three versions.
4. WHERE a faith reference appears, THE reference SHALL be embedded as character interiority or thematic texture — something Maya carries — rather than as a plot summary element.

---

### Requirement 7: Comparative Title Line

**User Story:** As the author, I want a specific author-comparison line included in all three versions, so that readers familiar with Kristin Hannah and Maggie O'Farrell immediately understand the literary register and emotional weight of this book.

#### Acceptance Criteria

1. THE Output File SHALL include the following exact line in all three versions: "For readers of Kristin Hannah and Maggie O'Farrell — a quiet, unflinching love story about what it costs to be known, and what it gives back."
2. THE comparative line SHALL appear at the top of each version, before the opening hook paragraph.
3. THE Output File SHALL NOT introduce any additional comparative title language beyond this single approved line.

---

### Requirement 8: Character and Story Accuracy

**User Story:** As the author, I want all copy to accurately reflect the characters, tone, and emotional arc of the manuscript, so that readers who purchase the book receive exactly the experience the copy promises.

#### Acceptance Criteria

1. THE descriptions SHALL name both leads — Maya Vasquez and Ethan Calloway — and establish their professional identities (Maya as curator/PhD candidate; Ethan as exhibition designer/photographer) where space allows.
2. THE descriptions SHALL frame Ethan's response to the disclosure as absence of flinching — a quiet, complete acceptance — rather than as heroism or rescue.
3. THE descriptions SHALL convey Maya's interiority: that she has built a managed, careful version of herself to show the world, and that Ethan is the first person to see past it.
4. THE descriptions SHALL reflect the novel's tone: emotionally precise, intelligent, not sentimental; resonant with readers who understand the arithmetic of trust.
5. THE descriptions SHALL NOT promise comic relief, a lighthearted tone, or an easy resolution — the emotional weight must be accurately represented.
6. THE descriptions SHALL reflect the novel's ending as an earned arrival — a wedding, a woman fully seen — without spoiling the disclosure scene or the threat arc.

---

### Requirement 9: Target Reader Voice and Register

**User Story:** As the author, I want the copy written in a register that speaks directly to the target reader — women 28–42 who are emotionally intelligent and know the particular cost of managing what you show the world — so that the right reader immediately recognises the book as being for her.

#### Acceptance Criteria

1. THE descriptions SHALL use emotionally precise, intelligent prose — neither clinical nor overwrought.
2. THE descriptions SHALL NOT use romance genre clichés (e.g., "steamy," "swoon-worthy," "perfect book boyfriend," "will leave you breathless") in any of the three versions.
3. WHEN describing Maya, THE descriptions SHALL convey specificity — she is a particular woman, not a symbol or archetype.
4. THE descriptions SHALL acknowledge the reader's own experience of guardedness, trust, and the decision to let someone fully in — without stating this explicitly; this should arrive through the emotional texture of the prose.

