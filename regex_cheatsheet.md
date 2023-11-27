**Metacharacters:**

| Symbol | Description | Example |
|---|---|---|
| `.` | Matches any single character (except newline) | `a.c` matches "abc" and "acc" but not "ac" |
| `*` | Matches zero or more occurrences of the preceding character or character class | `"ab"`* matches "ab", "abb", "abbb", etc. |
| `+` | Matches one or more occurrences of the preceding character or character class | `"ab"`+ matches "ab", "abb", "abbb", etc., but not "a" |
| `?` | Matches zero or one occurrence of the preceding character or character class | `"ab"`? matches "ab" or "a" |
| `{n}` | Matches exactly n occurrences of the preceding character or character class | `"ab"`{3} matches "ababab" |
| `{n,m}` | Matches at least n and at most m occurrences of the preceding character or character class | `"ab"`{2,4} matches "abab", "ababb", and "ababab" |
| `^` | Matches the beginning of a string | "^ab" matches strings that start with "ab", like "abacus" |
| `$` | Matches the end of a string | "us$" matches strings that end with "us", like "campus" |

**Character Classes:**

| Symbol | Description | Example |
|---|---|---|
| `[]` | Matches any single character from the specified set | `[abc]` matches "a", "b", or "c" |
| `[^]` | Matches any single character not in the specified set | `[^abc]` matches any character except "a", "b", or "c" |
| `\d` | Matches any digit (0-9) | `\d` matches "1", "2", "3", etc. |
| `\D` | Matches any non-digit character | `\D` matches "a", "b", "c", etc. |
| `\w` | Matches any alphanumeric character (a-z, A-Z, 0-9, or _) | `\w` matches "a", "b", "Z", "9", "_" |
| `\W` | Matches any non-alphanumeric character | `\W` matches whitespace, punctuation, and other non-alphanumeric characters |
| `\s` | Matches any whitespace character (space, tab, newline, etc.) | `\s` matches " ", "\t", "\n", etc. |
| `\S` | Matches any non-whitespace character | `\S` matches any character except whitespace |

**Grouping and Quantifiers:**

| Symbol | Description | Example |
|---|---|---|
| `( )` | Groups a subexpression, allowing for nested quantifiers and backreferences | `"ab(cd)*"` matches "abc", "abcd", "abcccd", etc. |
| `|` | Alternates between two or more subexpressions | `"cat|dog"` matches "cat" or "dog" |
| `?` | Makes the preceding quantifier non-greedy | `"ab"`*? matches "a" |
| `{n,}` | Matches at least n occurrences of the preceding character or character class, with no upper limit | `"ab"`{2,} matches "abab", "ababb", "ababab", etc. |

**Backreferences:**

| Symbol | Description | Example |
|---|---|---|
| `\1`, `\2`, etc. | Refers to the nth captured group | `(\w+)\1` matches strings like "hellohello" |

**Popular Commands:**

| Command | Description | Example |
|---|---|---|
| `grep` | Searches for text in files | `grep "pattern" filename` |
| `sed` | Stream editor for performing text transformations | `sed 's/pattern/replacement/g' filename` |
| `awk` | Pattern matching and data processing language | `awk '{print $1,$2}' filename` |
| `perl` | Powerful programming language with extensive text processing capabilities | `perl -pe 's/pattern/replacement/g' filename` |
| `python` | Versatile programming language with powerful text processing libraries | `python re.sub('pattern', 'replacement', 'string')` |

These are just some of the basics of regular expressions. For more in-depth information, please refer to the documentation for your specific programming language or regex tool.
