# Sponsor Pillow

Pillow is the Python imaging library. It is free, and it is one of the most
widely used packages in the Python ecosystem. This repository makes the case
for funding its maintenance.

## How widely Pillow is used

As of November 2026:

| Measure | Value | Source |
|---|---|---|
| PyPI downloads, last month | ~703 million | [pypistats.org](https://pypistats.org/packages/pillow) |
| PyPI downloads, last day | ~26.6 million | [pypistats.org](https://pypistats.org/packages/pillow) |
| Public GitHub repositories that depend on Pillow | 2,475,995 | [GitHub dependency graph](https://github.com/python-pillow/Pillow/network/dependents) |
| Packages that depend on Pillow | 39,385 | [GitHub dependency graph](https://github.com/python-pillow/Pillow/network/dependents) |

Downloads are mostly CI and container builds, so they overstate the number of
people. Dependents only count public repositories, so they understate it. Much
of Pillow's use is indirect, through packages such as matplotlib, torchvision
and Django.

## What it would be worth if every user paid

A thought experiment, not a pricing proposal. The user counts and prices below
are estimates, not measurements.

| Model | Assumption | MRR | ARR |
|---|---|---|---|
| Per developer | ~5M developers who use Pillow directly or knowingly, at $5/month | ~$25M | ~$300M |
| Per organisation, tiered | ~1M organisations: 900k small at $20, 90k mid-sized at $200, 10k enterprise at $2,000 per month | ~$56M | ~$670M |
| Per download | $0.001 per download | ~$0.7M | ~$8.4M |

That gives a rough range of **$25–60M MRR, or $300–700M ARR**.

Charging for Pillow would not raise that much. Most users would move to a fork
or another library, and Pillow's reach comes from being free and installed as a
dependency of other packages. The point is the scale of value Pillow provides
compared with the funding it receives.

## What funding pays for

The most practical measure is what the largest users would pay for the work
that keeps Pillow safe and current. At $2,000 a month, the 10,000 largest
organisations alone would come to about $240M a year. That work includes:

- **Security response.** Pillow parses untrusted image data in dozens of
  formats, partly in C. Maintainers triage private vulnerability reports,
  write and review fixes, request CVEs and publish advisories. A single
  release can include dozens of security fixes.
- **Releases and wheels.** Quarterly releases, with prebuilt wheels for
  Linux, macOS and Windows that bundle and update libjpeg, libpng, libtiff,
  libwebp, FreeType, Little CMS and other libraries.
- **Compatibility.** Support for new Python versions, including free
  threading, and new platforms.
- **Documentation**, including a [security threat
  model](https://pillow.readthedocs.io/en/latest/handbook/security.html).

## How to sponsor

- **GitHub Sponsors:** <https://github.com/sponsors/python-pillow>
- **Tidelift:** a subscription that pays maintainers and gives your
  organisation support for the packages you depend on.
  <https://tidelift.com/subscription/pkg/pypi-pillow>
