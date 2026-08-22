# comment-purge

A Claude Code skill that deletes the comments your code doesn't need.

Ask a model to "improve the comments" and it hands them back shorter.
Shorter redundancy is still redundancy. This one starts from delete. A
comment survives only if it gives a reason, states a contract, warns
about something non-obvious, or points to an issue, a spec, or a
fixture. The rest goes.

It works one file at a time, shows you a verdict for every comment, and
waits for your go-ahead before changing anything. It touches comments
only, never code, names, or formatting.

## Install

```
claude plugin marketplace add JacobJoergensen/comment-purge-skill
claude plugin install comment-purge@jacobjoergensen
```

Or, from inside a session:

```
/plugin marketplace add JacobJoergensen/comment-purge-skill
/plugin install comment-purge@jacobjoergensen
```

## License

MIT. See [LICENSE](LICENSE.md).
