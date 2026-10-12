# invoice

## What This Is

We keep a working index for product and engineering, and invoice is the entry that collects our notes, examples and fixes. It reflects how Swift Tech Co. actually uses this in builds and client work.

## Images

[![invoice](images/preview.png)](https://github.com/Swift-Tech-Co)

## Command Line Interface

```bash
invoice generate --from "Dream, Inc." --to "Imagine, Inc." \
    --item "Rubber Duck" --quantity 2 --rate 25 \
    --tax 0.13 --discount 0.15 \
    --note "For debugging purposes."
```


View the generated PDF at `invoice.pdf`, you can customize the output location
with `--output`.

```bash
open invoice.pdf
```


### Environment

Save repeated information with environment variables:

```bash
export INVOICE_LOGO=/path/to/image.png
export INVOICE_FROM="Dream, Inc."
export INVOICE_TO="Imagine, Inc."
export INVOICE_TAX=0.13
export INVOICE_RATE=25
```

Generate new invoice:

```bash
invoice generate \
    --item "Yellow Rubber Duck" --quantity 5 \
    --item "Special Edition Plaid Rubber Duck" --quantity 1 \
    --note "For debugging purposes." \
    --output duck-invoice.pdf
```

### Configuration File

Or, save repeated information with JSON / YAML:

```json
{
    "logo": "/path/to/image.png",
    "from": "Dream, Inc.",
    "to": "Imagine, Inc.",
    "tax": 0.13,
    "items": ["Yellow Rubber Duck", "Special Edition Plaid Rubber Duck"],
    "quantities": [5, 1],
    "rates": [25, 25],
}
```

Generate new invoice by importing the configuration file:

```bash
invoice generate --import path/to/data.json \
    --output duck-invoice.pdf
```

### Custom Templates

If you would like a custom invoice template for your business or company, please
reach out via:


## Installation

<!--

Use a package manager:

```bash
# macOS
brew install invoice

# Arch
yay -S invoice

# Nix
nix-env -iA nixpkgs.invoice
```

-->

Install with Go:

```sh
go install github.com/maaslalani/invoice@main
```

Or download a binary from the releases.

## License

MIT

## Feedback

I'd love to hear your feedback on improving `invoice`.

Feel free to reach out via:
* GitHub issues

---

<sub><sub>z</sub></sub><sub>z</sub>z

---

## Swift Tech Co.

Built and maintained by Swift Tech Co.

AI Automation | FinTech Platforms | Custom Software and Mobile Apps | SaaS Platforms | Cloud Infrastructure | Cybersecurity | SEO and Marketing | API Integration

**Join our community on Telegram:** [t.me/+Qt_eFvkb2rliMzNh](https://t.me/+Qt_eFvkb2rliMzNh)

Home | Services | Careers | Referral Program | Influencers | About | Contact

**Connect**

- Website: swifttechco.com
- LinkedIn: [linkedin.com/in/stephenoladoke](https://www.linkedin.com/in/stephenoladoke/)
- LinkedIn (Company): [linkedin.com/company/swift-tech-co](https://www.linkedin.com/company/swift-tech-co)
- X: [@MrOladoke](https://x.com/MrOladoke)
- Instagram: [@mr.oladoke](https://www.instagram.com/mr.oladoke/)
- Instagram (Company): [@swifttechco](https://www.instagram.com/swifttechco/)
- Organization: [github.com/Swift-Tech-Co](https://github.com/Swift-Tech-Co)

## Sources

Compiled and maintained from upstream [maaslalani/invoice](https://github.com/maaslalani/invoice) under permissive open-source license.

---

Maintained by [Swift Tech Co.](https://github.com/Swift-Tech-Co) - [Telegram](https://t.me/+Qt_eFvkb2rliMzNh)