+++
title = "ACME ADCS Server: Automate Your Certificate Issuance"
subtitle = "ACME Protocol for Your Windows PKI"
summary = "An RFC 8555-compliant server with ADCS as the backend."
description = "Automated certificate issuance for your ADCS environment. Secure, reliable, and without manual effort. Easy to set up. Test the product free of charge."
icon = "🔐"
weight = 1
+++

<div class="features-hero">
  <h1>ACME Protocol for Your Windows PKI</h1>
  <p class="lead">
    ACME-ADCS-Server connects any RFC 8555-compliant ACME client to your
    <strong>Microsoft® Active Directory Certificate Services</strong> infrastructure.
    Use familiar tools like <em>Certbot</em>, <em>win-acme</em>, or <em>ACME-PS</em>
    — and issue certificates directly from your own PKI.
  </p>
  <div class="mt-3 d-flex flex-wrap gap-2">
    <a href="https://glatzert.github.io/ACME-Server-ADCS/docs-v3.0/prereqs.html"
       class="btn btn-light">Quickstart Guide</a>
    <a href="https://github.com/glatzert/ACME-Server-ADCS"
       class="btn btn-outline-light">GitHub</a>
  </div>
</div>

---

## Manual Certificates? Not Anymore.

Certificates expire, get overlooked, or are issued incorrectly — and that's when it gets expensive.
Manual processes take time, introduce errors, and increase security risk.

ACME ADCS Server fully automates issuance and renewal via the ACME protocol.
It bridges the Microsoft Active Directory Certificate Authority and the Automatic Certificate
Management Environment (as popularised by Let's Encrypt), allowing any ACME (RFC 8555) compatible
client to issue certificates from your own PKI — giving you full control and security without
additional overhead.

---

## Why ACME-ADCS Server?

<div class="row row-cols-1 row-cols-sm-2 g-3 my-2">

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🧪</span>
      <h3>Free to Evaluate</h3>
      <p>ACME ADCS can be fully tested before any commitment. No risks, no obligations.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">👁️</span>
      <h3>Open Source</h3>
      <p>The entire solution is openly readable. Security reviews, audits, and internal assessments are straightforward.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🔗</span>
      <h3>Seamless Integration</h3>
      <p>Integrates directly into existing infrastructure — ideal for organisations with custom workflows or compliance requirements.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🛠️</span>
      <h3>Customisable</h3>
      <p>Open source means you can extend, integrate, or modify the solution to fit your internal processes perfectly.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">💶</span>
      <h3>Affordable Licensing</h3>
      <p>€1,500 one-time per corporate group — no extra charges per instance, user, server, or certificate.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">⭐</span>
      <h3>Proven & Active</h3>
      <p>Over 170 stars on GitHub, many satisfied customers worldwide, and ongoing active development.</p>
    </div>
  </div>

</div>

---

## Features at a Glance

<div class="row row-cols-1 row-cols-sm-2 row-cols-lg-3 g-3 my-2">

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🔒</span>
      <h3>RFC 8555 Compliant</h3>
      <p>Fully compliant ACME server — interoperable with any standards-conforming client without modification.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🔌</span>
      <h3>Any ACME Client</h3>
      <p>Certbot, win-acme, ACME-PS, acme.sh and many more clients work out of the box.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">✅</span>
      <h3>Multiple Challenge Types</h3>
      <p>Supports <code>http-01</code>, <code>dns-01</code>, and <code>tls-alpn-01</code> as well as experimental types for specialised scenarios.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🌐</span>
      <h3>DNS & IP Certificates</h3>
      <p>Certificates for DNS names and IP addresses (RFC 8738) — ideal for internal services without public DNS records.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🔑</span>
      <h3>External Account Binding</h3>
      <p>EAB enables binding ACME accounts to predefined permissions and corporate policies.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">📋</span>
      <h3>Certificate Profiles</h3>
      <p>Different ADCS templates, CA servers, or validity periods per use case — flexibly configurable.</p>
    </div>
  </div>

</div>

---

## Challenge Types in Detail

<h3 class="features-section-title">Supported Validation Methods</h3>

ACME-ADCS-Server supports the following challenge types for domain validation:

<ul class="badge-list">
  <li>http-01</li>
  <li>dns-01</li>
  <li>tls-alpn-01</li>
  <li class="experimental">dns-persist-01</li>
  <li class="experimental">device-attest-01</li>
</ul>

`http-01` and `dns-01` are the most widely used types and supported by virtually all ACME clients.
`tls-alpn-01` allows validation exclusively over TLS on port 443 per [RFC 8737](https://datatracker.ietf.org/doc/rfc8737/)
— no port 80 or DNS record required.

The experimental challenge types are still in the standardisation process.
`device-attest-01` enables client certificate issuance and is currently supported by Apple devices.

---

## Identifier Types

<h3 class="features-section-title">Supported Identifiers</h3>

<ul class="badge-list">
  <li>dns (RFC 8555)</li>
  <li>ip (RFC 8738)</li>
  <li class="experimental">permanent-identifier</li>
  <li class="experimental">hardware-module</li>
</ul>

Beyond classic DNS names, **IP addresses** can also be used as identifiers in certificates — a common
requirement in corporate networks where services are only reachable by IP.

---

## Certificate Profiles

<h3 class="features-section-title">Flexible Profile System</h3>

Profiles let you provide different configurations depending on the use case:

- **Automatic** — The server automatically selects the appropriate profile based on the identifier.
- **Client-selected** — The ACME client actively selects a profile, conforming to the [ACME Profiles Draft](https://datatracker.ietf.org/doc/draft-aaron-acme-profiles/01/).

This means you can use a different ADCS template for web server certificates than for IoT devices or
client certificates — all from a single installation.

---

## Additional Features

- **CAA Validation** — Checks Certification Authority Authorization records and method binding per [RFC 8657](https://datatracker.ietf.org/doc/rfc8657/).
- **External Account Binding (EAB)** — Bind accounts to corporate policies; [documentation](https://glatzert.github.io/ACME-Server-ADCS/docs/eab.html).
- **ADCS Auto-Enrollment** — Leverages the existing auto-enrollment configuration of your ADCS template.
- **Modern .NET** — Built on ASP.NET Core for a maintainable and extensible architecture.
- **SBOM** — Includes a Software Bill of Materials (CycloneDX) for transparency and compliance.

---

## Installation

Installation is deliberately kept simple. Everything you need is on GitHub.

1. Open the official [ACME ADCS GitHub repository](https://github.com/glatzert/ACME-Server-ADCS).
2. Follow the step-by-step installation guide provided there.
3. Adjust the configuration to match your existing ADCS environment.
4. Start the web server — done.

The documentation covers all details on setup, configuration, system requirements, and best practices.
You can start testing ACME ADCS immediately and only purchase a licence when you go into production.

<a href="https://glatzert.github.io/ACME-Server-ADCS/docs-v3.0/prereqs.html" class="btn btn-primary">Documentation (V3.0)</a>

---

## Licence & Pricing

<h3 class="features-section-title">Who can use the software free of charge?</h3>

<table class="pricing-table">
  <thead>
    <tr>
      <th>User group</th>
      <th>Condition for free use</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Private individuals</td>
      <td>No profit-making intent</td>
    </tr>
    <tr>
      <td>Educational providers</td>
      <td>Course fees &lt; €500 per semester</td>
    </tr>
    <tr>
      <td>Companies</td>
      <td>Total annual revenue &lt; €10 million</td>
    </tr>
    <tr>
      <td>Everyone</td>
      <td>Testing and evaluation purposes</td>
    </tr>
  </tbody>
</table>

For commercial use outside these boundaries, the licence fee is **€1,500 excl. VAT** with an
unlimited term. Maintenance and onboarding contracts can be arranged separately.

To request a quote, contact [thomas@th11s.de](mailto:thomas@th11s.de).

<div class="features-cta">
  <h2>Get Started</h2>
  <p>Connect your ADCS to the ACME protocol in just a few steps.</p>
  <a href="https://glatzert.github.io/ACME-Server-ADCS/docs-v3.0/prereqs.html"
     class="btn btn-light">Documentation (V3.0)</a>
  <a href="https://github.com/glatzert/ACME-Server-ADCS"
     class="btn btn-outline-light">GitHub Repository</a>
  <a href="mailto:thomas@th11s.de"
     class="btn btn-outline-light">Request a Licence</a>
</div>

---

## Voluntary Support

If ACME ADCS saves you time and prevents grey hairs, feel free to buy me a coffee.
No obligation — but caffeine keeps the development going:
[Thomas on PayPal](https://paypal.me/TGlatzer) ☕
