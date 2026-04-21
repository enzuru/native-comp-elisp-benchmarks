# native-comp-elisp-benchmarks — submit a PR with your own benchmark results!

This is a repo of elisp-benchmarks with native compilation run on different CPUs with different settings.

## High scores

We had to reset the high scores and exclude all scores that didn't use accurate Emacs settings (now documented below), so the below list may seem unusual if you are just looking at scores.

1. AMD Ryzen 9800X3D: 32.35s
2. AMD Ryzen 5700U: 54.94s

## Submit your own

Submit an org file with your benchmark results!

1. Install the `elisp-benchmarks` package from ELPA: https://elpa.gnu.org/packages/elisp-benchmarks.html
2. Set the following `elisp-benchmarks` variables so that we're testing the actual comp settings that your Emacs uses:
```lisp
(setq elb-speed native-comp-speed)
(setq elb-safety compilation-safety)
```
3. Run the `elisp-benchmarks-run` command to run the test and create the test results buffer
4. Save the buffer as `cpu-name.org` in the `cpu/` folder
5. Above the test results, Add a "Specs" section with your full CPU name, OS name + version, Emacs version, and `elisp-benchmarks` version (see existing CPU org files for an example)
6. You can optionally add a "Notes" section between "Specs" and "Results"

I am not trying to be extremely scientific by strictly controlling for all variables (OS, distro, build flags, motherboard, background services, etc). This is just meant to be fun and give us some rough perspective on how well Emacs is running with native compilation on different CPUs and settings.

If we get lots of results, we can start organizing by OS, Emacs version, etc.
