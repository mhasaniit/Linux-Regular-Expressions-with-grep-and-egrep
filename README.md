# Linux Regular Expressions with grep and egrep

## Overview

This project demonstrates the use of regular expressions in Linux using `grep` and `egrep` to search, filter, and analyze text data from multiple poem files.

The lab highlights pattern-matching techniques commonly used in system administration, scripting, cybersecurity, and log analysis.

## Objectives

* Search text files using grep
* Exclude matching lines
* Perform case-sensitive and case-insensitive searches
* Use anchors and wildcards
* Match patterns using regular expressions
* Compare grep and egrep functionality

## Environment Setup

```bash
mkdir ~/regex_practice
cd ~/regex_practice

cp ~/Downloads/opuses.zip .

unzip opuses.zip
```

## Commands Used

### Basic Search

```bash
grep "Captain" opus06.txt
```

### Inverted Search

```bash
grep -v "Captain" opus06.txt
```

### Case-Insensitive Search

```bash
grep -i "captain" opus06.txt
```

### Beginning-of-Line Anchors

```bash
grep "^I" opus01.txt
grep "^I " opus01.txt
```

### Wildcard Matching

```bash
grep "t.e" opus03.txt
```

### Multi-Character Pattern Matching

```bash
grep "w...e" opus03.txt
```

### Alternation

```bash
egrep "(wood|road)" opus01.txt
```

### End-of-Line Matching

```bash
grep "wall$" opus03.txt
```

### Blank Line Detection

```bash
grep "^$" opus03.txt
```

## Regular Expression Concepts

### Dot (.)

Matches any single character.

Example:

```regex
t.e
```

### Beginning Anchor (^)

Matches the start of a line.

Example:

```regex
^I
```

### Ending Anchor ($)

Matches the end of a line.

Example:

```regex
wall$
```

### Alternation (|)

Matches one pattern or another.

Example:

```regex
(wood|road)
```

## Skills Demonstrated

* Linux text processing
* Command-line filtering
* Pattern matching
* Regular expression fundamentals
* Log analysis techniques
* Bash terminal proficiency

## Real-World Applications

* System administration
* Security monitoring
* Log file analysis
* Automation scripts
* Data extraction
* DevOps workflows

## Outcome

I successfully applied regular expressions using grep and egrep to search, filter, and analyze text data, demonstrating foundational Linux skills used in administration, scripting, cybersecurity, and software engineering environments.
