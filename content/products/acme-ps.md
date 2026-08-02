+++
title = "ACME-PS"
summary = "RFC 8555 kompatible PowerShell Klientenbibliothek"
icon = "📜"
weight = 2
+++

<div class="features-hero">
  <h1>Zertifikate per PowerShell – automatisiert mit ACME</h1>
  <p class="lead">
    ACME-PS ist ein freies PowerShell-Modul, das alle Bausteine für die
    automatisierte Zertifikatsverwaltung über das <strong>ACME v2-Protokoll</strong>
    (RFC 8555) bereitstellt. Schreiben Sie eigene Skripte, um TLS-Zertifikate von
    Let's Encrypt, <em>ACME-ADCS-Server</em> oder jedem anderen ACME-kompatiblen CA zu beziehen.
  </p>
  <div class="mt-3 d-flex flex-wrap gap-2">
    <a href="https://www.powershellgallery.com/packages/ACME-PS/"
       class="btn btn-light">PowerShell Gallery</a>
    <a href="https://github.com/PKISharp/ACME-PS"
       class="btn btn-outline-light">GitHub</a>
  </div>
</div>

---

## Skripte statt Klickarbeit

Manuelle Zertifikatsanfragen sind fehleranfällig, zeitaufwändig und schlecht
automatisierbar. ACME-PS gibt Ihnen alle nötigen Cmdlets an die Hand, um den
gesamten Lebenszyklus — von der Kontoeröffnung bis zur Zertifikatsausstellung —
sauber in PowerShell-Skripten abzubilden und in bestehende Automatisierungspipelines
zu integrieren.

---

## Features auf einen Blick

<div class="row row-cols-1 row-cols-sm-2 row-cols-lg-3 g-3 my-2">

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">📋</span>
      <h3>RFC 8555 konform</h3>
      <p>Vollständige Umsetzung des ACME v2-Protokolls — interoperabel mit Let's Encrypt, ACME-ADCS-Server und anderen kompatiblen CAs.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🔑</span>
      <h3>RSA & ECDSA</h3>
      <p>Account-Keys und Zertifikats-Keys können als RSA oder ECDSA mit konfigurierbarer Schlüssellänge erstellt werden.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">✅</span>
      <h3>Mehrere Challenge-Typen</h3>
      <p>Unterstützt <code>http-01</code> und <code>dns-01</code> zur Domainvalidierung — wählbar je nach Infrastruktur.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🔗</span>
      <h3>SAN-Zertifikate</h3>
      <p>Mehrere Identifier (Subject Alternative Names) pro Zertifikat — ein Auftrag, ein Zertifikat für alle benötigten Domains.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">⛓️</span>
      <h3>Vollständige Zertifikatskette</h3>
      <p>Zwischenzertifikate werden automatisch in die Ausgabe einbezogen, sofern von der CA bereitgestellt.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">💾</span>
      <h3>Lokaler State</h3>
      <p>Alle Sitzungsdaten (Account, Nonces, Aufträge) werden in einem State-Objekt gehalten — einfach persistierbar und wiederverwendbar.</p>
    </div>
  </div>

</div>

---

## Installation

ACME-PS ist direkt über die PowerShell Gallery verfügbar und in Sekunden einsatzbereit:

```powershell
Install-Module -Name ACME-PS
```

Anschließend stehen alle Cmdlets zur Verfügung, um einen ACME-Workflow aufzubauen:

1. Account-Key generieren und beim ACME-Server registrieren
2. Identifiers (Domains) definieren und einen Order anlegen
3. Challenges lösen (`http-01` oder `dns-01`)
4. Zertifikats-Key erstellen und CSR senden
5. Fertiges Zertifikat (inkl. Kette) exportieren

Beispiele und Musterskripte finden sich direkt im [GitHub-Repository](https://github.com/PKISharp/ACME-PS/tree/main/samples).

---

## Weitere Informationen

- **Lizenz** — MIT, kostenfrei für jeden Einsatzzweck
- **119 Stars** auf GitHub, 14 Contributors, 23 Releases
- **Aktive Entwicklung** — regelmäßige Updates und Community-Beiträge

<div class="features-cta">
  <h2>Jetzt loslegen</h2>
  <p>ACME-PS steht kostenfrei auf der PowerShell Gallery und GitHub bereit.</p>
  <a href="https://www.powershellgallery.com/packages/ACME-PS/"
     class="btn btn-light">PowerShell Gallery</a>
  <a href="https://github.com/PKISharp/ACME-PS"
     class="btn btn-outline-light">GitHub-Repository</a>
  <a href="https://github.com/PKISharp/ACME-PS/tree/main/samples"
     class="btn btn-outline-light">Beispiele ansehen</a>
</div>
