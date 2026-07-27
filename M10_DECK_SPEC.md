# COMD 745 Module 10 — Deck Build Spec

**Module:** Clinical Considerations - Speech Recognition and Repair  
**Instructor:** Cara Vandergriff, MA, MS, CCC-SLP · University of South Carolina · Summer 2026  
**Deliverable:** three PowerPoint decks, 16:9, 13.333 x 7.5 inches.

## Palette — must match Modules 2 through 9

| Role | Hex |
|---|---|
| Background | `#F2EADA` |
| Headings, left rule | `#73000A` |
| Body text | `#676156` |
| Bullet glyphs | `#65780B` |
| Lecture number | `#A49137` |
| Captions | `#466A9F` |
| Footer band | `#D9C7A3` |

Georgia bold 26pt headings. Calibri 17 to 19pt body. Garnet vertical rule 0.28 in down the left edge of every slide. Honeycomb 3pt rule under each heading. Footer band across the bottom with her name at left and the slide number at right in garnet.

**Title slides:** the cover image fills the slide. It already contains the module title. Do not add a second title. Footer line only.

**Content slides:** figure across the top at full width, caption beneath in atlantic italic, bullets below at 13 to 14pt. Two slides are tables instead of figures.

**No speaker notes on any slide.** She records from a separate script.

**Do not rewrite the bullet text.** It is the exact display copy. Do not add a fourth bullet. Do not invent captions.

## Figures

Filenames refer to the `figures/` folder supplied with this spec.

---

# LECTURE 10.1

## Slide 1 — TITLE

Cover image `m10 cover.png` fills the slide. No added title text.

## Slide 2 — Where the Course Has Been

**Figure:** `DP_Fig1-1_speech_chain_ROTATED.png`  **FULL WIDTH**
**Caption:** The speech chain. Denes & Pinson, Figure 1-1.

**Bullets, exact text:**

- Modules 2 through 5 followed the signal out of the talker.
- Modules 6 through 9 followed it into the listener.
- Module 10 puts an automatic recognizer in the listener's place.

## Slide 3 — The Reading

**Figure:** `DP1_Fig8-1_PatternPlayback.png`  **FULL WIDTH**
**Caption:** The Pattern-Playback. Denes & Pinson, Figure 8-1.

**Bullets, exact text:**

- The assigned reading is Chapter 11, Automatic Speech Recognition, from your course text.
- It asks the question Module 9 asked: what in the acoustic signal identifies a sound?
- The answer came from building speech by hand and playing it to listeners.

## Slide 4 — Painted Speech

**Figure:** `DP1_Fig8-2_spectrogram_vs_painted.png`  **FULL WIDTH**
**Caption:** A natural spectrogram beside its painted equivalent. Figure 8-2.

**Bullets, exact text:**

- Formant patterns were painted onto film and converted back into sound.
- If a painted pattern is heard as a syllable, what was painted is sufficient to identify it.
- This isolated which acoustic features carry consonant identity.

## Slide 5 — The Second Formant Transition

**Figure:** `DP1_Fig8-6_formants_upward_downward_transition.png`  **FULL WIDTH**
**Caption:** Formants with various degrees of upward and downward transition. Figure 8-6.

**Bullets, exact text:**

- The second formant glides into the following vowel rather than starting at a fixed frequency.
- Changing the direction and extent of that glide changes the consonant that is heard.
- Nothing else in the pattern is altered.

## Slide 6 — Transition and Place of Articulation

**Figure:** `DP1_Fig8-8_F2transition_place_of_articulation.png`  **FULL WIDTH**
**Caption:** Second formant transition and place of articulation. Figure 8-8.

**Bullets, exact text:**

- Six synthetic patterns are heard as pa, ta, ka and ma, na, nga.
- Patterns sharing a place of articulation share a second formant transition.
- The pairs differ only in what precedes the vowel: silence for plosives, a low buzz for nasals.

## Slide 7 — Context

**Figure:** `DP1_Fig8-12_importance_of_context.png`  **FULL WIDTH**
**Caption:** The importance of context. Figure 8-12.

**Bullets, exact text:**

- Listeners resolve ambiguous sounds using the words around them.
- This is the top-down support you measured on yourself in the Module 9 lab.
- The recognizer in the next lecture does not have it.

---

# LECTURE 10.2

## Slide 1 — TITLE

Cover image `m10 cover.png` fills the slide. No added title text.

## Slide 2 — The Comparison

**Figure:** `Screenshot 2026-07-27 122552.png`  **FULL WIDTH**
**Caption:** The Align tab. Pause threshold and tier selection are left at their defaults.

**Bullets, exact text:**

- Mrs. Jones produced the eleven recordings you transcribed in Module 9.
- The same audio file goes to Open Brain AI for automatic alignment.
- Same speaker, same recordings. Only the listener changes.

## Slide 3 — What the Software Returns

**Figure:** `Screenshot 2026-07-27 122751.png`  **FULL WIDTH**
**Caption:** Word and sentence tiers for the two sentence clips.

**Bullets, exact text:**

- The TextGrid populates below the spectrogram, one tier for words and one for sentences.
- Each detected word carries a start time and an end time.
- Those timestamps are how you match each clip to the right row in your worksheet.

## Slide 4 — What the Machine Returned

**Full-width table.** Header row garnet fill, sandstorm text.
Shade these data rows at 20 percent horseshoe (zero-indexed): [3, 6, 7, 8]

| Clip | Target | Format students had | Machine returned |
|---|---|---|---|
| 1 | rake | four options | Rink |
| 2 | train | four options | cane |
| 3 | storm | four options | scum |
| 4 | corn | four options | corn |
| 5 | feed | two options | bees |
| 6 | trait | two options | crane |
| 7 | knee | no options | knee |
| 8 | double | no options | double |
| 9 | jacket | no options | jacket |

Caption beneath in atlantic italic: *Shaded rows are the four the recognizer identified correctly.*

## Slide 5 — This Is Not a New Finding

**Figure:** `CHART_expectation_vs_classdata.png`  **FULL WIDTH**
**Caption:** Denes & Pinson Table 8-1 plotted with COMD 745 Module 9 results.

**Bullets, exact text:**

- Denes and Pinson ran this experiment: give listeners a set of words to choose from, then vary how many.
- Two choices, 87 percent correct. Four, 69. Thirty-two, 39. Two hundred fifty-six, 14.
- Your class: four printed options, 82.5 percent. Two options, 63.2. No options, 39.6.
- Nothing about the speech changed in either case. Only the size of the guess changed.

## Slide 6 — The Original Table

**Figure:** `DP1_Table8-1_expectation_vocabulary_size.png`  **FULL WIDTH**
**Caption:** Denes & Pinson, Table 8-1. The effect of expectation on speech recognition.
**Ties back to:** Module 1, information theory

**Bullets, exact text:**

- The column on the right is percent of words correctly identified.
- A listener choosing between two words is not doing the same task as one choosing among 256.
- Both are called intelligibility testing. Both produce a number. The numbers are not comparable.

## Slide 7 — Where the Two Listeners Diverge

**Figure:** `CHART_openresponse_human_vs_machine.png`  **FULL WIDTH**
**Caption:** Open-response items only. No answer choices for either listener.

**Bullets, exact text:**

- The software identified 4 of the 9 single words: corn, knee, double, and jacket.
- On the first sentence it scored 50.0 percent against a class average of 49.3.
- On the second it scored 66.7 percent against a class average of 40.7.
- It wins on some items and loses on others. Neither listener is reliable alone.

## Slide 8 — Where Each Listener Failed

**Figure:** `CHART_sentences_word_by_word.png`  **FULL WIDTH**
**Caption:** Every target word in the two sentences. Garnet is the student mean.

**Bullets, exact text:**

- No student in the scored sample recovered the final cluster in jumps. The software did.
- That cluster reduces to /s/ versus /t/: same place of articulation, differing only in manner.
- Sibilant energy is high frequency and low intensity, so it is among the first information lost.
- Thirteen of eighteen students got quick. The software returned it fused with the following word.

## Slide 9 — Why Run It At All

**Figure:** `OBAI BROAD BAND LAB TASK FORMANTS.png`  **FULL WIDTH**
**Caption:** A time-aligned spectrogram of the lab stimuli.
**Ties back to:** Module 5, reading a spectrogram

**Bullets, exact text:**

- The software has no access to meaning, so it cannot resolve a disagreement for you.
- What it does give you is a time-aligned spectrogram of the exact segment in question.
- Continuous frication at the end of a word points to /s/. A closure and release burst points to /t/.
- The disagreement tells you where to look. The acoustic record tells you what happened.

## Slide 10 — Template Matching

**Figure:** `DP2_Fig11-2_recognizer_block_diagram.png`  **FULL WIDTH**
**Caption:** Basic structure of an automatic speech recognizer. Figure 11-2.

**Bullets, exact text:**

- rake became Rink. train became cane. feed became bees. trait became crane.
- Every one is a real English word rather than noise.
- The recognizer returns the stored template closest to the input, and every stored template is a word.

## Slide 11 — The Lab

**Figure:** `lab task scrn sht pg1 1-2.png`  **FULL WIDTH**
**Caption:** The Module 10 lab worksheet.

**Bullets, exact text:**

- Run Mrs. Jones's eleven recordings through Open Brain AI and record what it returns.
- Compare three transcriptions per clip: the target, your Module 9 answer, and the software's.
- Calculate percent intelligibility for both listeners at the word level and the sentence level.
- Complete her clinical statement and Frenchay intelligibility ratings from your own numbers.

---

# LECTURE 10.3

## Slide 1 — TITLE

Cover image `m10 cover.png` fills the slide. No added title text.

## Slide 2 — Mrs. Jones: Clinical Profile

**Full-width table.** Header row garnet fill, sandstorm text.
Shade these data rows at 20 percent horseshoe (zero-indexed): [2]

| Frenchay area | Rating |
|---|---|
| Intelligibility, single words | markedly reduced |
| Intelligibility, sentences | markedly to severely reduced |
| Intelligibility, conversation | moderately reduced, better than single words |
| Tongue, elevation and lateral | markedly impaired |
| Tongue, alternate movement | markedly to severely impaired |
| Palate, in speech | markedly impaired |
| Respiration, in speech | markedly impaired |

Caption beneath in atlantic italic: *Her intelligibility rows are completed by students in the lab. TORGO does not publish a diagnosis for individual speakers, so none is stated here.*

## Slide 3 — Her Profile Predicted the Results

**Figure:** `Ryalls_Fig10-1_PDP_interactive_activation.png`  **FULL WIDTH**
**Caption:** Signal and stored knowledge meeting during word recognition.

**Bullets, exact text:**

- Her assessment rates connected speech better than single words.
- Student sentence scores were higher than isolated word scores on the same recordings.
- Her articulation did not change between conditions. The information available to the listener did.

## Slide 4 — What an Intelligibility Score Requires

**Figure:** `CHART_student_accuracy_by_format.png`  **FULL WIDTH**
**Caption:** The same nine words, three response formats.

**Bullets, exact text:**

- A percent-correct score describes a talker, a listener, a response format, and a room together.
- The same recordings produced 82.5 percent and 39.6 percent from the same students in one sitting.
- A number reported without its conditions cannot be compared to anything.

## Slide 5 — Individual Variation and Baselines

**Figure:** `OBAI_DDK_irregular_rate_rhythm.png`  **FULL WIDTH**
**Caption:** An irregular diadochokinetic pattern.

**Bullets, exact text:**

- The Module 8 diadochokinetic lab produced a range of rates across this class on an identical task.
- A norm describes a sample. A baseline describes your patient.
- When a patient cannot be compared to a norm, compare them to themselves over time.

## Slide 6 — We Keep Reaching for the Spelling

**Figure:** `DP1_Fig8-12_importance_of_context.png`  **FULL WIDTH**
**Caption:** Denes & Pinson, Figure 8-12. Letters removed from a sentence, and how many guesses each one took.
**Ties back to:** Module 1

**Bullets, exact text:**

- You transcribed sounds all term, and every worksheet asked you to write them down as letters.
- Letters are not sounds. English has 26 letters and roughly 44 sounds, and the spelling hides that.
- When you cannot identify a sound, the pull is to write the nearest word instead. So does the software.
- That pull is what every task in this course was designed to interrupt.

## Slide 7 — How to Get the Text Out of the Way

**Figure:** `ExtIPA_chart_2025_full.png`  **FULL WIDTH**
**Caption:** The extended IPA. Notation for productions that no ordinary spelling covers.
**Ties back to:** Modules 9 and 10 labs

**Bullets, exact text:**

- Single words remove the sentence, so meaning cannot fill the gap for you.
- Automatic transcription removes meaning entirely, since the software has none.
- The extended IPA gives you symbols for sounds that are not any word at all.
- None of these is more real than conversation. Each one hides a different crutch from you on purpose.

## Slide 8 — Sound Behaves Differently From Print

**Figure:** `DP_Fig1-1_speech_chain_ROTATED.png`  **FULL WIDTH**
**Caption:** The speech chain. Everything in the middle is sound, and none of it holds still.
**Ties back to:** Module 1

**Bullets, exact text:**

- A word on a page sits still. You can look back at it. A spoken word is gone as you finish saying it.
- Say the word permanence. By the time you reach the end, the beginning is already gone, and has to be.
- You can rap on a box and hear whether it is empty. Sound tells you about the inside of things.
- That is why a voice tells you so much about a person, and why we can measure a vocal tract without opening one.

## Slide 9 — The Feedback Link

**Figure:** `DP_Fig1-1_feedback_link_CROP.png`  **FULL WIDTH**
**Caption:** The feedback link. Denes & Pinson, Figure 1-1.

**Bullets, exact text:**

- The feedback link is how a talker detects a mismatch between what they intended and what they produced.
- Monitoring runs below awareness. Awareness is a separate event.
- A patient who can hear the mismatch has a reason to work on it, which is where a target comes from.

## Slide 10 — Getting a Clean Measure: The Probe

**Figure:** `lab task scrn sht pg1 1-2.png`  **FULL WIDTH**
**Caption:** The lab worksheet works the same way: fixed targets, no cues, scored the same each time.
**Ties back to:** Module 10 lab

**Bullets, exact text:**

- A probe is a short set of untested targets, roughly ten items, run at the start of a session.
- No cues, no models, no reminders, no encouragement. It will feel uncomfortable to withhold them.
- It tells you what the patient does without you, which is the only thing that predicts carryover.
- Match the probe to the task that established baseline so the two are comparable over time.

## Slide 11 — Why Probe Data Beats Cued Data

**Figure:** `CHART_student_accuracy_by_format.png`  **FULL WIDTH**
**Caption:** The same principle you measured on yourself: remove the support and the score changes.
**Ties back to:** Module 9 and 10 labs

**Bullets, exact text:**

- Performance recorded with maximum support describes the session, not the patient.
- A goal written around level of cueing is difficult to track and does not survive discharge.
- Probes are quick, which spares you documenting a session while also running it.
- Your patient does not take you home, to the book club, or to work. Measure what travels.

## Slide 12 — Repair: Sharing Context

**Figure:** `DP_Fig1-1_speech_chain_ROTATED.png`  **FULL WIDTH**
**Caption:** Shared context supports the linguistic link on both ends of the chain.
**Ties back to:** Module 1, the speech chain

**Bullets, exact text:**

- Ask a caregiver to transcribe what their loved one says to the prompt, tell me about a day at the beach.
- Run it again with a picture of a beach scene that both of them can see.
- Speech and content on the speaker side get richer, and the listener can track what is being referred to.
- Most useful when the breakdown is at the language level, as in aphasia.

## Slide 13 — Repair: Targeted Repair and Topic Marking

**Figure:** `Ryalls_Fig10-1_PDP_interactive_activation.png`  **FULL WIDTH**
**Caption:** Repair works on the same signal and knowledge system perception runs on.
**Ties back to:** Module 9, top-down support

**Bullets, exact text:**

- Targeted repair: the listener repeats back everything they heard and leaves only the gap blank, so the speaker repairs one word instead of the whole utterance. Most useful in dysarthria.
- Topic marking: note the topic when the speaker begins. If they stall, you can say, you were telling me about the grocery store. Most useful in dementia.
- Offer repair carefully. A wrong guess creates a second breakdown on top of the first.
- Speech is redundant. Language is not. People who stutter report that what they were about to say rarely matches what a listener supplies.

## Slide 14 — The Evidence That Is Not in a Paper

**Figure:** `DP_Fig1-1_feedback_link_CROP.png`  **FULL WIDTH**
**Caption:** The feedback link. Denes & Pinson, Figure 1-1.
**Ties back to:** Module 8, the feedback link

**Bullets, exact text:**

- Ask the patient directly: when to help, how to help, what to avoid.
- Ask what they want their condition called, and what language they find inaccurate or upsetting.
- Reframe for buy-in without obscuring or softening the clinical information.
- This is internal evidence. It exists only in the person in front of you.
