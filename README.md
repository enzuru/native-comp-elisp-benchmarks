# native-comp-elisp-benchmarks — submit a PR with your own benchmark results!

This is a repo of elisp-benchmarks with native compilation run on different CPUs with different settings.

## High scores

1. AMD Ryzen 7950X: 14.36s
2. Apple M4: 16.01s
3. AMD Ryzen 5900X: 20s
4. Intel i3 14100F: 20.87s
5. Apple M3: 24.13s
6. Intel i5 1350P: 25.23s
7. AMD Ryzen 5700G: 25.51s
8. Intel Core i9-11900K: 26.42s
9. Apple M2: 28.94s
10. Intel i7-1355U: 29.31s

## Submit your own

Submit an org file with your benchmark results!

0. Install the `elisp-benchmarks` package from ELPA: https://elpa.gnu.org/packages/elisp-benchmarks.html
1. Run the `elisp-benchmarks-run` command to run the test and create the test results buffer
2. Save the buffer as `cpu-name.org` in the `cpu/` folder
3. Above the test results, Add a "Specs" section with your full CPU name, OS name + version, Emacs version, and `elisp-benchmarks` version (see existing CPU org files for an example)
4. You can optionally add a "Notes" section between "Specs" and "Results"

It's OK to adjust Emacs settings to get a higher benchmark score. Just document what settings you used.

I am not trying to be extremely scientific by strictly controlling for all variables (OS, distro, build flags, motherboard, background services, etc). This is just meant to be fun and give us some rough perspective on how well Emacs is running with native compilation on different CPUs and settings.

If we get lots of results, we can start organizing by OS, Emacs version, etc.
