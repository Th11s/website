+++
title = "ACME-PS"
summary = "RFC 8555-compatible PowerShell client library"
icon = "📜"
weight = 2
+++

<div class="features-hero">
  <h1>Certificates via PowerShell — Automated with ACME</h1>
  <p class="lead">
    ACME-PS is a free PowerShell module that provides all the building blocks for
    automated certificate management over the <strong>ACME v2 protocol</strong>
    (RFC 8555). Write your own scripts to obtain TLS certificates from
    Let's Encrypt, <em>ACME-ADCS-Server</em>, or any other ACME-compatible CA.
  </p>
  <div class="mt-3 d-flex flex-wrap gap-2">
    <a href="https://www.powershellgallery.com/packages/ACME-PS/"
       class="btn btn-light">PowerShell Gallery</a>
    <a href="https://github.com/PKISharp/ACME-PS"
       class="btn btn-outline-light">GitHub</a>
  </div>
</div>

---

## Scripts Instead of Manual Work

Manual certificate requests are error-prone, time-consuming, and hard to automate.
ACME-PS gives you all the cmdlets you need to model the full certificate lifecycle —
from account creation to certificate issuance — cleanly in PowerShell scripts and
integrate it into your existing automation pipelines.

---

## Features at a Glance

<div class="row row-cols-1 row-cols-sm-2 row-cols-lg-3 g-3 my-2">

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">📋</span>
      <h3>RFC 8555 Compliant</h3>
      <p>Full implementation of the ACME v2 protocol — interoperable with Let's Encrypt, ACME-ADCS-Server, and other compatible CAs.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🔑</span>
      <h3>RSA & ECDSA</h3>
      <p>Account keys and certificate keys can be created as RSA or ECDSA with configurable key sizes.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">✅</span>
      <h3>Multiple Challenge Types</h3>
      <p>Supports <code>http-01</code> and <code>dns-01</code> for domain validation — selectable based on your infrastructure.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🔗</span>
      <h3>SAN Certificates</h3>
      <p>Multiple identifiers (Subject Alternative Names) per certificate — one order, one certificate for all required domains.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">⛓️</span>
      <h3>Full Certificate Chain</h3>
      <p>Intermediate certificates are automatically included in the output if provided by the CA.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">💾</span>
      <h3>Local State</h3>
      <p>All session data (account, nonces, orders) is held in a state object — easy to persist and reuse across script runs.</p>
    </div>
  </div>

</div>

---

## Installation

ACME-PS is available directly from the PowerShell Gallery and ready to use in seconds:

```powershell
Install-Module -Name ACME-PS
```

Once installed, all cmdlets are available to build an ACME workflow:

1. Generate an account key and register it with the ACME server
2. Define identifiers (domains) and create an order
3. Solve challenges (`http-01` or `dns-01`)
4. Create a certificate key and submit the CSR
5. Export the finished certificate (including the full chain)

Sample scripts and detailed examples are available in the [GitHub repository](https://github.com/PKISharp/ACME-PS/tree/main/samples).

---

## Further Information

- **Licence** — MIT, free for any use case
- **119 stars** on GitHub, 14 contributors, 23 releases
- **Actively maintained** — regular updates and community contributions

<div class="features-cta">
  <h2>Get Started</h2>
  <p>ACME-PS is freely available on the PowerShell Gallery and GitHub.</p>
  <a href="https://www.powershellgallery.com/packages/ACME-PS/"
     class="btn btn-light">PowerShell Gallery</a>
  <a href="https://github.com/PKISharp/ACME-PS"
     class="btn btn-outline-light">GitHub Repository</a>
  <a href="https://github.com/PKISharp/ACME-PS/tree/main/samples"
     class="btn btn-outline-light">View Examples</a>
</div>
