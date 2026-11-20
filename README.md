# Build a Business

A 50-minute classroom game that teaches 2nd to 5th graders what an entrepreneur does. You and your team are forming a new company to sell a new product. You can invest 10 coins in different priorities, see what happens, change the plan and try again.

**Live demo:** https://davidjette.github.io/find-your-path/

Made by David Jette for a parent-led session at an elementary school. It is free for teachers, parents and volunteers to use and adapt. See [License](#license).

## How the game works

Kids sit in teams of four to seven. Each team invents a company and gets 10 coins and three sheets:

| Sheet | What it buys |
|---|---|
| **Build It** | A better product (engineer, designer, testing and so on) |
| **Tell People** | Customers hearing about it (posters, ads, free samples, an optional celebrity) |
| **Protect It** | Cover when things go wrong (insurance, lawyer, backup plan) |

Teams place their coins, and the presenter types each team's totals into the game. The scoring is kept secret until the first reveal:

1. **Customers** are the smaller of Build and Tell. A great product nobody heard about gets no customers, and neither does a famous product that breaks.
2. **Celebrity news.** The game picks one superstar (teams that hired them double their customers) and one "oops" (teams that hired them lose 2).
3. **Risk Die.** Something always goes wrong. If the roll is bigger than a team's Protect total, the team loses the difference.

In Year 2 each team gets 10 coins plus one for every customer it kept, and three minutes to change its plan. The scoreboard adds both years. The lesson is in the second try: teams see what went wrong and fix it.

## What is in the repo

| File | Purpose |
|---|---|
| `index.html` | The game, shown on a projector: slides, team list, Year 1 and Year 2 reveals, Risk Die, scoreboard and countdown timers |
| `sheets.html` | Four printable pages per team: Build It, Tell People, Protect It and a scorecard |
| `notes.html` | Presenter notes for a phone: a timed outline, team sizes, a rules cheat sheet and backups |
| `img/` | Portraits of the six celebrities |

There is no build step, no server and no dependencies. Each page is a single HTML file with its styles and script inline.

## Run it

Open `index.html` in a browser, or use the live demo. Once loaded it works without the internet.

- Arrow keys or the space bar move through the slides.
- The four buttons at the top (Purple, Orange, Indigo, Blue) are four separate groups, so one presenter can run several sessions in a day. Rename them on the Teams tab.
- Scores are saved in the browser's local storage on that device. Nothing is sent anywhere.
- "Load practice teams" on the Teams tab fills in four sample teams for a dry run.
- Print `sheets.html` on letter paper, one set per team. Pennies fit the coin spots.

## Make it your own

- **The story slides.** Slides 3 to 8 tell the author's own story (his job, a company he started and a project that failed). Replace them with yours. The slides are a plain list near the top of the script in `index.html`, under `EDIT YOUR SLIDES HERE`.
- **Business ideas and company names.** Edit the two "Pick your" slides in the same list.
- **Celebrities.** Edit the `CELEBS` list in `index.html` and the matching block in `sheets.html`, and add a square-ish portrait to `img/`.
- **Risk Die events.** Edit the `EVENTS` list, one line per die face.
- **Timers.** Change `timer:6` and `timer:3` on the two GO slides (minutes).
- **Things to buy.** Edit the rows in `sheets.html`.

## License

Text, design and code are licensed under [Creative Commons Attribution-NonCommercial 4.0](LICENSE) (CC BY-NC 4.0). You may use, copy and adapt the game for classrooms, clubs, camps and other non-commercial teaching, as long as you credit "Build a Business by David Jette" and link to this repo.

The portraits in `img/` are not covered by that license. See the credits below.

## Image credits

The portraits are thumbnails of the lead images of each person's English Wikipedia article, from Wikimedia Commons. Each is marked public domain there.

| Person | Source |
|---|---|
| George Washington | Portrait by Gilbert Stuart |
| Cleopatra | Bust in the Altes Museum, Berlin (photo: Louis le Grand) |
| William Shakespeare | Portrait attributed to John Taylor |
| Amelia Earhart | Photograph by Underwood & Underwood |
| Albert Einstein | Photograph by Oren Jack Turner |
| Leonardo da Vinci | Portrait attributed to Francesco Melzi |
