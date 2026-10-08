# onetrace — issues

This repository is where you report problems with, and ask questions about, the **onetrace** Python packages:

- [`onetrace`](https://pypi.org/project/onetrace/): the SDK (recording, `diff`, `localize`, `reproduce`, `anchor`, `sign`)
- [`onetrace-verify`](https://pypi.org/project/onetrace-verify/): the reference verifier

It contains no code. The documentation is at [oneproof.dev/onetrace](https://oneproof.dev/onetrace/), and each release's notes and files are under **Releases**. Open an issue using the **Issues** tab.

## Security problems: do not open a public issue

If you think you've found a security problem, for example a record the verifier accepts when it shouldn't, a way to make a changed record verify, or anything that could mislead someone relying on a verification result, **email onetrace@oneproof.dev** instead. Please include the same details as for a bug (below). You'll get a reply, and a fix before any public discussion.

## Reporting a bug

Please include:

1. **Versions:** the output of `pip show onetrace onetrace-verify`, your Python version, and your operating system.
2. **What you ran:** the exact command or the smallest code that shows the problem.
3. **What happened:** the full output, including any traceback, and the exit code (`echo $?`, or `$LASTEXITCODE` in PowerShell).
4. **What you expected** instead.
5. **A run folder, if the problem involves one.** Attach it if you can (zip it). Remove anything confidential first. Receipts contain digests and your stage names, constants and assertions, and `artifacts/` contains your pipeline's actual outputs.

## Before you report

- **A refusal ends with a `fix:` line and a `see:` line.** The [errors page](https://oneproof.dev/onetrace/errors.md) explains each one.
- **What each verdict and exit code means** is on the [verdicts page](https://oneproof.dev/onetrace/verdicts.md).
- **What a record, a signature or an anchor does not show** is listed on the [non-claims page](https://oneproof.dev/onetrace/non-claims.md).
- **A folder holds one run.** Use a new folder for each run.

## Questions and ideas

Questions about how to integrate onetrace, and feature ideas, are welcome as issues too. Please add the `question` or `idea` label if you can.

## Licence

onetrace is licensed under Apache-2.0.
