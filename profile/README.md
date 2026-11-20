## marqius-wkhtmltopdf: a maintained, drop-in wkhtmltopdf replacement

The wkhtmltopdf project was archived on 2 January 2023. **marqius-wkhtmltopdf** is a maintained, Rust-based wkhtmltopdf alternative from Simple AI LLC for applications that launch the `wkhtmltopdf` executable. Keep your library, HTML templates and PDF calls; point your library's binary setting at marqius-wkhtmltopdf.

### Tested in public

- **[wkhtmltopdf parity suite](https://github.com/marqiushq/wkhtmltopdf-parity)**: the same HTML documents through wkhtmltopdf 0.12.6 and marqius-wkhtmltopdf on every release, on x86-64 and ARM64, with every PDF compared and every result published, misses included. Run it on your own templates; nothing is uploaded.
- **[Integration examples](https://github.com/marqiushq/marqius-wkhtmltopdf-examples)**: runnable HTML-to-PDF examples for 14 wkhtmltopdf libraries, among them python-pdfkit, django-wkhtmltopdf, KnpLabs Snappy, laravel-snappy, wicked_pdf, PDFKit, Rotativa.AspNetCore and go-wkhtmltopdf.

### Resources

- [marqius-wkhtmltopdf](https://marqius.com/wkhtmltopdf/): product, plans and a 30-day trial
- [Migration guide for each wkhtmltopdf library](https://marqius.com/blog/wkhtmltopdf-deprecated-alternatives/)
- [Docker images](https://hub.docker.com/r/marqius/wkhtmltopdf) for Debian, Alpine and slim deployments, on amd64 and arm64

marqius-wkhtmltopdf is commercial software from Simple AI LLC. The parity suite is open source under the MIT licence, and its test documents are public domain (CC0).
