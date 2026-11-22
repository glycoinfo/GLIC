# Contributing to the GLIC website

The GLIC website (<https://glic.glycoinfo.org>) is built from this repository. Anyone can suggest a new
resource or a correction, and you do not need to know how the site is built to do so.

## Suggest a resource or a correction

**Easiest:** [open an issue](https://github.com/glycoinfo/GLIC/issues/new) describing the change. You can
also email the [GLIC mailing list](https://groups.google.com/g/glycoinformatics-consortium-glic).

**If you are comfortable with GitHub:** edit the page's Markdown file directly on GitHub (pencil icon) and
open a pull request. A GLIC maintainer reviews every change before it is published.

For a new software tool or database, please include:

- the resource name and its official website;
- a one- or two-sentence description written for someone who has not used it;
- its main use case and the data it handles (for example MS, NMR, glycan structures, glycan arrays);
- a documentation or source-code link, if there is one;
- a contact person or address;
- your relationship to the resource (for example developer, user), if any.

## Where things are

| To change | Edit |
| --- | --- |
| Software list | `software/index.md` |
| Databases list | `database/index.md` |
| Homepage | `index.md` |
| Main menu | `_data/navigation.yml` |
| Meetings, Seminars | `meetings/index.md`, `seminars/index.md` |
| Requests form page, Wish List page | `wishList/index.md`, `toolsList/index.md` |
| Board members and mailing list | `aboutus/index.md` |
| Colours, spacing, buttons | `assets/css/style.scss` |
| Header and footer of every page | `_layouts/default.html` |

Every push to the `master` branch is published automatically by GitHub Pages within a few minutes.

## Entry template

Copy this into `software/index.md` or `database/index.md`, in the place you want it to appear. Keep the
rows that apply and write **Not specified** when you do not know a value, rather than guessing.

```md
### Resource name

One sentence saying what the resource does.

| **Use case** | What a researcher would use it for |
| **Data** | e.g. MS, NMR, glycan structures, glycan arrays |
| **Type** | Web application / Standalone software / Software library / Database |
| **Access** | <https://example.org> |
| **Source code** | <https://github.com/example/example> |
| **Documentation** | <https://example.org/docs> |
| **License** | e.g. MIT, CC-BY-4.0, or Not specified |
| **Status** | e.g. stable, under development |
| **Contact** | Name: <name@example.org> |

Longer description, publications and funding (optional).
```

Database entries can also use **Search options**, **Data download**, **Coverage** and **Curated** rows (see
existing entries). The contents list at the top of each page updates itself from the `###` headings.

Do not rename an existing `###` heading unless you have to: its text forms the link (`#anchor`) that other
sites may use to point at the entry.

## Keeping information accurate

- Only publish what has been checked. If a licence, status or link has not been confirmed, say
  **Not specified** or leave it out.
- A working link does not show that a tool is maintained, and an old repository does not show that it is
  abandoned. Ask the developers rather than inferring either.
- "Last reviewed by GLIC" (when a maintainer last checked an entry) is not the same as "last updated by the
  developers". If you record a review date, use the real date of the check, never a date taken from Git.
- Do not add automatic status badges or uptime checks: they suggest someone is monitoring the resource.

## Periodic review (for maintainers)

A light review every few months keeps the site trustworthy. Suggested checklist:

- [ ] Homepage and menu links open the expected pages.
- [ ] Meetings: anything listed under "Upcoming meetings" is really upcoming; past events moved down.
- [ ] Seminars: new series added to `seminars/index.md`.
- [ ] RDF page: the endpoint still answers a query; update the date in the "Availability" line.
- [ ] Requests form and Wish List spreadsheet still load, also on a phone.
- [ ] Software and Databases: "Access" links still work; report broken ones to the entry's contact.

## Previewing the site on your computer (optional)

Not needed for small text changes. With Ruby installed, create a file called `Gemfile` (not committed) containing:

```ruby
source "https://rubygems.org"
gem "github-pages", group: :jekyll_plugins
```

then run `bundle install` once and `bundle exec jekyll serve`, and open <http://localhost:4000>.
