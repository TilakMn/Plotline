# Plotline

**Open-source product and project management that adapts to how your team actually works.**

Plotline is for business owners, product managers and project managers. You organize work
as products, each with one or more projects. When you create a project you choose its
methodology (Agile, Waterfall, Hybrid or Scaled), and the backlog, boards, roadmap and
rules adapt to it.

> **Status: early prototype.** Plotline is a working demo that saves data in your browser.
> Shared team workspaces and accounts are on the roadmap. Feedback and contributions are welcome.

## Try it

- **Online:** open the live demo (see *Publish the demo* below once GitHub Pages is on).
- **Locally:** download `index.html` and open it in Chrome, Edge, Firefox or Safari.

The demo opens with a sample product, *Greenbox*, so you can explore straight away.
Use **Restore sample** in the top bar to reset it.

## What it does

### Methodology-driven projects
| Methodology | What changes |
|---|---|
| **Agile** | Epics and user stories, ranked backlog, sprints, sprint board, Now/Next/Later roadmap |
| **Waterfall** | Requirements and work packages, phases with signed gates, locked baseline, change requests |
| **Hybrid** | Phase gates for requirements, sprints for the stories inside them |
| **Scaled** | Features between epics and stories, program board across teams, dependency warnings |

### Prioritization, several ways
The same backlog can be analysed with **MoSCoW**, **RICE**, **WSJF**, **MOST** and an
**as-is / to-be process map**. A **Compare** view flags the stories where the methods
strongly disagree, which are usually the priority conversations worth having.

### Honest forecasting
Instead of one guessed deadline, Plotline simulates the remaining work 3,000 times and shows:
- the most likely finish, a date that is safe to promise (80%), and an almost-certain date (95%)
- the chance of hitting any date you pick
- **what can be delivered by a date**: stories sorted into safe, possible and unlikely
- the effect of **scope growth** (new work added each sprint)
- a **confidence label** that says how much to trust the forecast, and why

What-if settings (team speed, predictability, sprint length, scope) change the forecast only,
never the project.

### Teams and deadlines
- Managers see everything; members see only the work assigned to them
- Deadlines on stories, epics and projects, marked red when overdue
- Assignees, reporters, comments and acceptance criteria on every issue
- Mobile-friendly layout with bottom navigation

## Tech

A single self-contained HTML file: plain JavaScript and CSS, no build step, no framework.
Fonts load from Google Fonts. Data is kept in the browser's `localStorage`.

## Roadmap

- [ ] Shared workspaces with sign-in (self-hostable backend such as PocketBase or Supabase)
- [ ] Docker image for one-command self-hosting
- [ ] Split the single file into modules with tests
- [ ] "My work" page and deadline reminders
- [ ] Forecast history and accuracy tracking
- [ ] Burn-up chart with a forecast cone
- [ ] Import from CSV and Jira

## Publish the demo with GitHub Pages

1. In your repository, open **Settings > Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Save. After a minute the demo is live at `https://<your-username>.github.io/<repository-name>/`.

## Contributing

Contributions of any size are welcome: bug reports, ideas, design feedback and code.
See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

Plotline is licensed under the [GNU Affero General Public License v3.0](LICENSE).
You can use, change and share it freely. If you run a modified version as a service
for others, you must publish your changes under the same license.
