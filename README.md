# readability-score-javascript
Simple vanilla JavaScript rewrite of the [textstat.py](https://github.com/shivam5992/textstat/) library.

Pass any (English) text to the function, and it returns an object with:

* Flesch Reading-Ease
* Flesch-Kincaid Grade
* SMOG Grade
* Coleman-Liau Index
* Automated Readability Index
* Linsear Write
* Rix
* Reading time (seconds)
* Median grade

For example, the object for

```
This is not a scientific result in any way. Heck, the whole concept of readability escapes scientific scrutiny (just look at the number of different tests with different values!). If you want to modify it, you could use the average grade as well (take both rounded down and rounded up to get the grade spread). Or you could find what grade is the most common in the whole spread and use that instead.
```

would look like this:

```
{
  automatedReadabilityIndex: 8.84,
  colemanLiauIndex: 8.24,
  fleschKincaidGrade: 8.28,
  fleschReadingEase: 68.18,
  linsearWriteFormula: 11.38,
  medianGrade: 9,
  readingTime: 17.51,
  rix: 3,
  smogIndex: 11.7
}
```

Read [this article](https://www.simoahava.com/analytics/calculate-readability-scores-for-content/) for an example on how to deploy this on a website with [Google Tag Manager](https://tagmanager.google.com/).
