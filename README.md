# native-comp-elisp-benchmarks — submit a PR with your own benchmark results!

This is a repo of elisp-benchmarks with native compilation run on different CPUs.

## High scores

1. AMD Ryzen 5900X: 31.73s
2. Apple M1: 40.37s
3. Intel i7-9750H: 40.39s

## Submit your own

Submit an org file with your benchmark results!

0. Install the `elisp-benchmarks` package from ELPA: https://elpa.gnu.org/packages/elisp-benchmarks.html
1. Run the `elisp-benchmarks-run` command to run the test and create the test results buffer
2. Save the buffer as `cpu-name.org` in the `cpu/` folder
3. Above the test results, Add a "Specs" section with your full CPU name, OS name + version, Emacs version, and `elisp-benchmarks` version (see existing CPU org files for an example)
4. You can add a "Notes" section too between "Specs" and "Results"

I am not trying to be extremely scientific by strictly controlling for all variables (OS, distro, build flags, motherboard, background services, etc). This is just meant to be fun and give us some rough perspective on how well Emacs is running with native compilation on different CPUs.

If we get lots of results, we can start organizing by OS, Emacs version, etc.
