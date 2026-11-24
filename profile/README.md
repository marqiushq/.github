## marqius-wkhtmltopdf: the maintained wkhtmltopdf replacement

**Rebuilt from scratch.**

The command line is wkhtmltopdf's, refined over twelve years and relied on by a great many apps: the same command, the same options, the same HTML templates. Everything behind it is new: one file, no X server, no Qt, no libraries to install, built the modern way:

- released in public, every build with its checksum beside it ([latest release](https://github.com/marqiushq/marqius-wkhtmltopdf/releases/latest))
- every build attestable in one command:
  `gh attestation verify marqius-wkhtmltopdf-linux-x86_64 -R marqiushq/marqius-wkhtmltopdf`
- every release tested in public, on real documents, misses included

The command line proved itself for a decade. The rebuild keeps it running on today's systems (Ubuntu 26.04, Debian 13, Alpine, Heroku-24) and tomorrow's.

**wkhtmltopdf turns HTML into PDF, and a great many apps rely on it** for invoices, receipts, reports and labels. Its project was archived in January 2023, and Debian 13 and Ubuntu 26.04 no longer include it.

**marqius-wkhtmltopdf is a drop-in replacement.** It takes the same command, the same options and the same HTML templates, so your code does not change. It is one program, kept up to date, with nothing else to install, and much faster than wkhtmltopdf.

```bash
curl -fsSL https://marqius.com/marqius-wkhtmltopdf.sh | bash
brew install marqiushq/tap/marqius-wkhtmltopdf
docker run --rm -v "$PWD:/data" marqius/wkhtmltopdf invoice.html invoice.pdf
```

### Start here

- **[marqius-wkhtmltopdf](https://github.com/marqiushq/marqius-wkhtmltopdf):** what it is, how to install it and how to switch your library in one step.
- **[Examples](https://github.com/marqiushq/marqius-wkhtmltopdf-examples):** working examples for 14 libraries, from python-pdfkit and Snappy to wicked_pdf and Rotativa.

### Tested in public, misses included

- **[Parity suite](https://github.com/marqiushq/wkhtmltopdf-parity):** the same documents through wkhtmltopdf and marqius-wkhtmltopdf on every release, every PDF compared. Run it on your own templates.
- **[Library tests](https://github.com/marqiushq/wkhtmltopdf-library-tests):** the test suites of 15 wkhtmltopdf libraries, run with both programs, with signed results.
- **[Signed builds](https://github.com/marqiushq/marqius-wkhtmltopdf/attestations):** check that any download is the file GitHub built, in one command.

### Install it your way

- **[apt, dnf and apk](https://github.com/marqiushq/packages):** signed repositories for Debian, Ubuntu, Rocky, Red Hat, Fedora, Amazon Linux and Alpine.
- **[Homebrew](https://github.com/marqiushq/homebrew-tap):** Apple silicon Macs and Linux.
- **[GitHub Actions](https://github.com/marqiushq/setup-marqius-wkhtmltopdf):** one step on any runner, and a [parity check](https://github.com/marqiushq/wkhtmltopdf-parity-check) that compares your PDFs on every pull request.
- **[Docker](https://hub.docker.com/r/marqius/wkhtmltopdf):** images for amd64 and arm64, from a 10 MB download.

marqius-wkhtmltopdf is commercial software from [Simple AI LLC](https://marqius.com), free for 30 days. The examples, the test suites and the GitHub Actions are open source. Questions: hello@marqius.com.
