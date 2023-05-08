# Ngram Type


## About

I learned **Touch Typing** and [**Colemak DH**](https://colemakmods.github.io/mod-dh/) keyboard layout from scratch to improve my typing speed/accuracy/comfort. The journey included training with Ngrams dataset. Ngram refers to sequence/grouping of characters, and they're usually ranked to describe the common ones. Historically, ngrams are used in Crytography to decrypt messages. Nowadays, they have many applications, for classifying spam messages, as auto-completion or spell-checking tool, etc. Technically, Ngrams are words also, and vice versa.

In Josh Kaufman's [**The First 20 Hours**](https://first20hours.com/) book (one of his personal challenges is to learn Colemak in 20 hours in which he succeeded), he used ngrams mostly as well as practice dataset:

> Human languages, including English, follow a power law curve called Zipf’s law: a very small set of words makes up the vast majority of actual usage. Based on an analysis of The Brown Corpus (1964), a 1 million-word collection of 500 modern English documents, only 135 words account for 50 percent of all English usage. The word "the" itself accounts for 7.5 percent, while "of" accounts for 3.5 percent.

Hence, Ngrams are practical and valuable training data. The better you're able to type these sequences of characters, the faster you'll be able to type in general. However, there's no free online typing website that integrates ngrams. And the typing tests on various websites are usually based on common English words. This project aims to provide a training ground for boosting typing speed/accuracy by focusing your performance in small and controlled phrases/chunks. Perfect training after all required perfect training on small set of data.

This **Ngram Type** project name was inspired by [**Amphetype**](https://github.com/webiest/amphetype) and [**MonkeyType**](https://monkeytype.com/). I've ported some of the ideas in the Amphetype also into this project.


## Features
* Data source could be chosen, based on the most common ngrams/words. Source settings' are independent with each other: lesson generator and minimum performance settings are set for each data source.
* Custom data source could be inputted using the `Custom` link.
* Lessons could be customized and generated on-the-fly by varying the `Scope`, `Combination`, and `Repetition` settings; you'll immediately see the effect on the generated lesson. Old lessons on the same data source selected will be overridden once you update these settings. Once you completed the lessons, the data will start again at the beginning, but will be re-shuffled.
* The minimum WPM/Accuracy required could be adjusted depending on your skill level, could be updated even at the mid-part of the lessons. You could not proceed to next lesson unless you have met those minimum performance. Average WPM refers to the average of all the WPMs in the current round of lessons that passed the threshold, which will be reset every round of lesson, so that old/historical averages will not affect the new ones. Average WPM is then a good indicator of your current speed which could be used for adjusting the performance thresholds in the next round of lessons.
* Has sound effects: correct key, wrong key, or failed the minimum WPM/Accuracy set.
* Has color indicator if you typed a wrong key.
* Timer will start/stop depending in your typing activity. It's included just for tracking.
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


## Effective Practice
The ultimate aim of Ngram Type is to have good typing performance in real-life scenarios, or in typing sites like [Monkey Type](https://monkeytype.com/)/[10 Fast Fingers](https://10fastfingers.com/). To excel in these contexts, need to practice with `Repetition=1` and `Combination=max` where `max` usually is between `20-40`. That's what I did also before since I really want to improve my **Monkey Type** performance. Monkey Type has similar settings to that of `Repetition=1` and `Combination=200` (i.e. using the **Top 200** English words). But of course, having `Combination=200` in Ngram Type is not realistic, even athletes practice mostly in short bursts/sessions instead of full game.

So, here's one good training pattern (increasing `Combination`, and decreasing `Repetition` through time):

```
Repetition=3, Combination=3
Repetition=3, Combination=4
...
Repetition=3, Combination=10

---

Repetition=2, Combination=3
Repetition=2, Combination=4
...
Repetition=2, Combination=10

---

Repetition=1, Combination=3
Repetition=1, Combination=4
...
Repetition=1, Combination=10
```

Then, increase the **Speed** threshold on each round (each set of `Repetition` and `Combination`) based on your running average speed, or once you feel that the current set becomes easy/comfortable for you. Likewise, you could also aim up to `Combination=15` or `Combination=20` instead of `Combination=10` only. This guarantees building good muscle memory and continual progress.

Increasing `Combination` and decreasing `Repetition` (which re-shuffles the data ordering as well) makes the exercise harder, which your muscle will adapt eventually. You should start mastering the Bigrams/Trigrams first since they are the building blocks of the English words, so you could have good performance even in `Top 1000` words. Although most typing sites only test for `Top 200` words. But training those Bigrams/Trigrams really well is a good investment. And if you always aim for 100% Accuracy at the expense of speed, eventually your speed will catch up since you will build "good" muscle memory and correcting mistakes is costly. Likewise, if you have low accuracy, you will build a "bad" muscle memory.

You could start with Top 50 bigrams/trigrams/tetragrams/words first. Then, move to Top 100, Top 150, and Top 200 as your performance improves.

## Hosted Version
You could access the online version using GitHub Pages:
- https://ranelpadon.github.io/ngram-type/

## Translations
- Russian
  - Project Page:
    - https://github.com/aleuxser/ngram-type-ru/
  - Hosted Version:
    - https://aleuxser.github.io/ngram-type-ru/
- French
  - Project Page:
    - https://github.com/edmundlam/ngram-type-fr/
  - Hosted Version:
    - https://edmundlam.github.io/ngram-type-fr/

