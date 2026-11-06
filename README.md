# Listening Test Simulator

A full Listening practice test: four parts and 40 questions, heard once, with 2 minutes to check at the end, as on computer.

Part of the [IELTS Study Suite](https://github.com/Apurba94/ielts-study-suite): 100 free study apps for IELTS. This one is for the IELTS Academic and General Training test. It works offline, as a Windows program or in the browser.

## Download and run

- **Windows:** download `Listening Test Simulator.exe` from the [latest release](https://github.com/Apurba94/ielts-listening-test/releases/latest) and open it. Nothing to install. It opens in its own window and saves your progress in your user folder.
- **Browser:** open it online in the suite's web edition at https://ielts-study-suite.vercel.app/apps/ielts-listening-test/ . Progress stays in that browser.
- **From source:** `python launcher.py` (Python 3.10 or later, no packages needed).

## What it does

A full Listening practice test in the order of the real one: an everyday call, a talk, a discussion and an academic lecture, each heard once, with time to check at the end, as on computer. This practice test has about 30 questions rather than 40, so the raw score is scaled to 40 before it is converted to an approximate band with the published guide table.

Sections: Test, Band table, Progress, About.

## How to use it

1. Use headphones, find a quiet place and allow 30 minutes.
2. Press **Start the test**. For each part, read the questions, then press Play once.
3. Move between parts with the buttons at the top, then press Finish the test.
4. The band is approximate: real tests have 40 questions and their own conversion tables.

## Good to know

- All questions, passages, recordings and definitions were written for this suite. None are official IELTS questions. For official practice, use the materials on ielts.org and from the test partners.
- It follows IELTS as delivered on computer in 2026. Formats change, so check ielts.org before your test.
- Listening uses the voices installed on your computer, which sound less natural than real test recordings.
- Feedback on writing and speaking counts what a program can count honestly, such as length and linking words. It is not an IELTS band score. Band conversions for Listening and Reading are approximate.
- Not endorsed by or affiliated with the British Council, IDP or Cambridge University Press & Assessment. IELTS is a registered trademark of its owners.

## For developers

The app is plain HTML and JavaScript in `web/`, run by a small Python launcher that serves it on 127.0.0.1 only and needs a secret token for saving. Tests: `node --test "tests/*.test.js"` (29 tests) and `python -m unittest discover -s tests`. Build the .exe with `python build_exe.py`.

Built with AI assistance (Claude Code). MIT licence. By JANIN A APURBA.
