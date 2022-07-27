# Non-deterministic `pnpm` install
Reproduction of a non-deterministic `pnpm` install.

Using `pnpm` 7.6.0 & Node.js v18.6.0 on MacOS Monterey (12.4), MacBook Pro 2021 (M1).

**Steps to reproduce:**
1. Clone the repository: `git clone git@github.com:JanJakes/pnpm-nondeterministic-install.git`.
2. Run `pnpm install`.
3. Repeat running `pnpm install` until you see `Packages: +1`.
4. Repeat running `pnpm install` until you see `Packages: -1`.

In steps 3. and 4. the following keeps being added to and removed from `pnpm-lock.yaml`:

<img width="1033" alt="Screen Shot 2022-07-27 at 9 10 06" src="https://user-images.githubusercontent.com/141436/181184226-57174c22-ace8-4e4a-bda8-ff21a2e607fd.png">
