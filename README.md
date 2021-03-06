# Ngram Type


## About

I'm recently practicing **Touch Typing** and [**Colemak DH**](https://colemakmods.github.io/mod-dh/) keyboard layout to improve my typing speed/accuracy. Ngram refers to sequence/grouping of characters, and they're usually ranked to describe the common ones. Historically, ngrams are used in Crytography to decrypt messages. Nowadays, they have many applications, for classifying spam messages, as auto-completion or spell-checking tool, etc. Technically, ngrams are words also, and vice versa.

In Josh Kaufman's [**The First 20 Hours**](https://first20hours.com/) book (one of his personal challenges is to learn Colemak in 20 hours in which he succeeded), he used ngrams mostly as well as practice dataset:

> Human languages, including English, follow a power law curve called Zipf’s law: a very small set of words makes up the vast majority of actual usage. Based on an analysis of The Brown Corpus (1964), a 1 million-word collection of 500 modern English documents, only 135 words account for 50 percent of all English usage. The word "the" itself accounts for 7.5 percent, while "of" accounts for 3.5 percent.

Hence, ngrams are practical and very useful training data. The better you're able to type these sequences of characters, the faster you'll be able to type in general. However, there's no free online typing website that integrates ngrams. And the typing tests on various websites are usually based on common English words. This project aims to provide a training ground for boosting typing speed/accuracy by focusing your performance in small and controlled phrases/chunks. Perfect training after all required perfect training on small set of data.

This **Ngram Type** project name was inspired by [**Amphetype**](https://github.com/webiest/amphetype) and [**MonkeyType**](https://monkeytype.com/). I've ported some of the ideas in the Amphetype also into this project.


## Features
* Data source could be chosen, based on the most common ngrams/words. Source settings' are independent with each other: lesson generator and minimum performance settings are set for each data source.
* Custom data source could be inputted using the `Custom` link. Defaults to [**pangrams**](https://en.wikipedia.org/wiki/Pangram) if no custom data is set. Pangrams are useful for training with all letters of the alphabet.
* Lessons could be customized and generated on-the-fly by varying the `Combination` and `Repetition` settings; you'll immediately see the effect on the generated lesson. Old lessons on the same data source selected will be overridden once you update these settings. Once you completed the lessons, the data will start again at the beginning, but will be re-shuffled.
* The minimum WPM/Accuracy required could be adjusted depending on your skill level, could be updated even at the mid-part of the lessons. You could not proceed to next lesson unless you have met those minimum performance. Average WPM refers to the average of all the WPMs in the current round of lessons that passed the threshold, which will be reset every round of lesson, so that old/historical averages will not affect the new ones. Average WPM is then a good indicator of your current speed which could be used for adjusting the performance thresholds in the next round of lessons.
* Has sound effects: correct key, wrong key, or failed the minimum WPM/Accuracy set.
* Has color indicator if you typed a wrong key.
* Timer will show once you start typing, for added tracking. There's no time limit though, you practice at your own pace.
* Settings are saved in your browser, and will be auto-loaded when you revisit/reload the page.

## Sample Lessons
Using the **Top 50 Words** as sample source, you could have sample lessons/patterns like this:
- Setting: `Combination=1`, `Repetition=3`
    - Output: **the the the**

- Setting: `Combination=2`, `Repetition=3`
    - Output: **the and the and the and**

- Setting: `Combination=3`, `Repetition=3`
    - Output: **the and of the and of the and of**

- Setting: `Combination=3`, `Repetition=1`
    - Output: **the and of**

- Setting: `Combination=3`, `Repetition=2`
    - Output: **the and of the and of**


## Hosted Version
You could access the online version using GitHub Pages:
- https://ranelpadon.github.io/ngram-type/
