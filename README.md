# linger2ibex

Convert your Linger-formatted psycholinguistics stimuli to [Ibex](https://github.com/addrummond/ibex) format! Input is a [Linger items file](http://tedlab.mit.edu/~dr/Linger/readme.html); output is a `.js` file to go in `data_includes` in your Ibex setup.

This is a standalone Python 3 script with no dependencies. It is designed to be run on the command line.

Usage:
```{python}
python3 linger2ibex.py ../path/to/linger/file.txt > ../path/to/output/file.js
```

By default, this script outputs your stimuli into a self-paced reading (SPR) setup. You can modify this by passing in your desired experiment type as the second argument. The options are currently `DashedSentence` (for SPR) and `AcceptabilityJudgment`.

I've only tested this on my own files. Let me know by filing an issue if it's not working for you!

Limitations:
* Only supports true/false type questions.
