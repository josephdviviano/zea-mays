zea-mays
--------

Usage:

    zea-mays template.yml output

A password candidate generator for when you can remember:

+ the base word(s) you used, but not capitalization or symbol replacement
+ the prefixes and/or postfixes you commonly use for your passwords

It outputs all of the candidates in plain text.

This can be useful if you tend to make long passwords with symbols mixed case alphanumerics, but you also cheat and re-use the same themes / words in your passwords, and you seem to have forgotten one of them over the years.

**example**

The included template is for a fictional person who: 

+ favourite musician was David Bowie
+ favourite hero was Batman
+ favourite piece of cinema was Airbud 
+ commonly added `SECRET` to the beginning of some of their passwords 
+ sometimes either their birthyear, or some symbols, to the end 
+ sometimes used mixed capitalization, and sometimes replaced vowels with numbers (e.g., A == 4).

`zea-mays` will generate a paltry 2340 possible passwords to test with the above rules, like so:

```
...
b0w1e
SECRETb0w1e1990
SECRETb0w1e!!!1
SECRETb0w1e???
SECRETb0w1e*
B0w1e
SECRETB0w1e1990
SECRETB0w1e!!!1
SECRETB0w1e???
SECRETB0w1e*
boW1e
SECRETboW1e1990
SECRETboW1e!!!1
SECRETboW1e???
SECRETboW1e*
BoW1e
...
```

**template.yml**

This file is required to generate your password candidates. You must list your input base words as a list, as well as a list of prefixes and postfixes.

Note that you must put certian symbols in quotes so that `yaml` interprets them correctly (see `template.yaml`).

