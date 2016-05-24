zea-mays
--------

Usage:

    zea-mays template.yml output

A password candidate generator for when you can remember:

+ the base word(s) you used, but not capitalization or symbol replacement
+ the prefixes and/or postfixes you commonly use for your passwords

It outputs all of the candidates in plain text for a brute force attack.

This can be useful if you tend to make long passwords with symbols mixed case alphanumerics, but you also cheat and re-use the same themes / words in your passwords, and you've forgotten one of them over the years.

**example**

The included template is for a fictional person whose favourite musician was David Bowie, favourite hero was Batman, and favourite piece of cinema was Airbud. This person thought it was cute to prepend 'SECRET' to some of their passwords, and sometimes either their birthdate, or some symbols, to passwords over the years. They also used mixed capitalization and sometimes replaced vowels with numbers (e.g., A == 4).

`zea-mays` will generate a paltry 2340 possible passwords to test with the above rules.

**template.yml**

This file is required to generate your password candidates. You must list your input base words as a list, as well as a list of prefixes and postfixes.

Note that you must put certian symbols in quotes so that `yaml` interprets them correctly (see `template.yaml`).

