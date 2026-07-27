# Lecture 10.2 — Automatic Speech Recognition

Recording script.

## Slide 1

This is lecture two of Module ten. We are going to hand the same recordings you transcribed by ear to a piece of software and compare what happens.

## Slide 2

Here is the setup. [pause] Mrs. Jones produced the eleven recordings you worked with in Module nine. Nine single words and two sentences. This week those exact files go into Open Brain AI for automatic alignment. [pause] What you are looking at is the Align tab. Language is set to English. The pause threshold is a quarter second. Sentences and Words are both checked. None of that gets touched. The point is that we changed nothing about the audio and nothing about the settings. The speaker is the same, the recordings are the same, the quality is the same. Only the listener changed.

## Slide 3

After it processes, this is what comes back. [pause] It is called a TextGrid, and it sits underneath the spectrogram. One tier for individual words, one tier for full sentences. [pause] Each detected word carries a start time and an end time. Those timestamps are how you match a clip to a row in your worksheet, which matters because all eleven clips are in one audio file.

## Slide 4

Now the results. [pause] Nine single words down the left. The target, the format you had in Module nine, and what the software returned. [pause] It got four. Corn, knee, double, and jacket. [pause] It missed five. Rake came back as Rink. Train as cane. Storm as scum. Feed as bees. Trait as crane. [pause] Hold onto those five for a minute, because how it failed is more interesting than that it failed.

## Slide 5

Before we go further, I want to show you something. [pause] Denes and Pinson ran an experiment where they gave listeners a set of words to choose from and then varied how many words were in the set. Two choices, listeners scored eighty seven percent. Four choices, sixty nine. Thirty two choices, thirty nine. Two hundred fifty six choices, fourteen percent. [pause] Now here is your class. Four printed options, eighty two and a half percent. Two options, sixty three. No options at all, just under forty. [pause] Nothing about the speech changed in either study. In theirs, the recordings were identical across conditions. In yours, the recordings were identical across conditions. The only thing that changed was how big the guess was.

## Slide 6

Here is the original table. [pause] The column on the right is percent of words correctly identified. [pause] A listener choosing between two words is not doing the same task as a listener choosing among two hundred fifty six. Both get called intelligibility testing. Both produce a percentage. Those percentages are not comparable to each other, and if you put one of them in a chart without saying which task produced it, nobody downstream can use it.

## Slide 7

Back to the comparison. [pause] The software identified four of the nine single words. On the first sentence it scored fifty percent, and the class average was forty nine point three. Essentially a tie. On the second sentence the software scored sixty six point seven and the class averaged forty point seven. [pause] So it wins some and loses some. There is no condition where one of them is reliably better than the other.

## Slide 8

Look at where each one failed, word by word. [pause] On the sentence about the fox, not one student in the scored sample recovered the final cluster in jumps. The software got it. [pause] Why is that cluster hard? Jumps ends in m, p, s. Jumped ends in m, p, t. So the whole decision comes down to s versus t. Those two share a place of articulation. They are both alveolar. The only thing separating them is manner, one is a fricative and one is a stop. [pause] And the s carries very little acoustic energy, concentrated way up high in frequency, which makes it among the first information to go when a signal degrades. It sits at the end of an unstressed word at the end of a sentence, which is exactly where speakers reduce and listeners stop attending. [pause] Meanwhile thirteen of eighteen students got quick, and the software fused it with the word after it and returned something that is not a word at all.

## Slide 9

So why run it. [pause] The software has no access to meaning. It cannot tell you which of you is right, because it does not know what the sentence is about. [pause] What it does give you is this. A time-aligned spectrogram of the exact segment in question. You can select the disputed word and look at it. [pause] If you see continuous frication at the end of that word, that points to an s. If you see a closure and then a release burst, that points to a t. [pause] The disagreement between you and the machine tells you where to look. The acoustic record tells you what actually happened. That is the workflow.

## Slide 10

One more thing about how it fails. [pause] Rake became Rink. Train became cane. Feed became bees. Trait became crane. [pause] Every single one of those is a real English word. Not a nonsense syllable. Not garbage. A real word. [pause] That is because of how it works. It compares what came in against stored examples of every word it knows and returns the closest match. Every stored example is a real word, so every error is a real word. [pause] Which means the output always looks confident, even when it is completely wrong. Keep that in mind when a piece of software hands you a clean transcript.

## Slide 11

That brings us to the lab. [pause] You are going to run Mrs. Jones's eleven recordings through Open Brain AI yourself and record what it gives you. [pause] Then you compare three transcriptions for each clip: the target, what you wrote in Module nine, and what the software returned. [pause] You calculate percent intelligibility twice at the word level and twice at the sentence level, once for you and once for the machine. Then you complete her clinical statement and fill in her Frenchay intelligibility ratings using your own numbers. [pause] Everything you need is in the worksheet, and the walkthrough steps are at the top.
