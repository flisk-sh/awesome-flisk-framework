# Contributing

Thanks for helping make the TDK resource catalog more useful. This repository is a curated directory for developers using or extending [TDK](https://github.com/flisk-sh/flisk).

## What belongs here

Suggest a public resource that is directly useful to people working with TDK, such as an official project, example, extension, integration, tutorial, article, gist, talk, or supporting tool. The catalog aims to include useful work from the wider community as well as official TDK resources.

Before proposing an entry, check that it:

- Has a public, working, canonical URL.
- Has a clear connection to TDK and a concise description of its use.
- Is not already listed under another heading.
- Is labeled accurately as **Official**, **Community**, **External project**, or **Archived**.
- Is maintained or still useful; mark inactive repositories as **Archived**.

For gists specifically:

- The gist must be public and reachable without login.
- It must be about TDK or the local-development problems TDK claims to solve.
- Maintainer or website-contributor gists are **Official**; third-party gists are **Community** only after a maintainer checks they are not spam.
- Do not include paywalled or deleted gists.
- If a gist duplicates an official article, link the article as the primary resource and describe the gist as a “short note.”
- List each gist's stable individual permalink, one approved topic, its label, and the core/docs page or command it maps to. Gists are secondary to core documentation.

Submissions that are inaccessible, unrelated, duplicative, or primarily promotional may be declined. Maintainers may ask for context or move an entry to a more suitable section.

## Entry format

Add one Markdown bullet under the most relevant heading in `README.md`:

```markdown
- [Resource name](https://example.org): one-sentence description. **Community**
```

Use **Official** for resources maintained by `flisk-sh`, **Community** for independently maintained TDK resources, **External project** for a tool or technology used by TDK, and **Archived** for discontinued repositories. Use the appropriate label for the resource rather than assuming every project in the TDK organization is currently maintained.

## Submit a change

For a small suggestion or a question, [open an issue](https://github.com/flisk-sh/awesome-tdk-framework/issues). To add or correct links directly:

1. Fork the repository and create a branch.
2. Edit `README.md` and follow the entry format above.
3. Check the URL, description, label, and section. Remove any duplicate entry.
4. Open a pull request describing the resource and why it belongs in the catalog.

There is no build step. Keep changes focused on the resource catalog, and do not add generated files, assets, or automation.
