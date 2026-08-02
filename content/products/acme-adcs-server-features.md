+++
title = "ACME-ADCS-Server – Funktionen"
subtitle = "ACME-Protokoll für Ihre Windows-PKI"
summary = "Alle Funktionen des ACME-ADCS-Servers im Überblick."
+++

<link rel="stylesheet" href="/css/features.css">

<div class="features-hero">
  <h1>ACME-Protokoll für Ihre Windows-PKI</h1>
  <p class="lead">
    Der ACME-ADCS-Server verbindet jeden RFC-8555-kompatiblen ACME-Client mit Ihrer
    <strong>Microsoft® Active Directory Certificate Services</strong>-Infrastruktur.
    Nutzen Sie vertraute Tools wie <em>Certbot</em>, <em>win-acme</em> oder <em>ACME-PS</em>
    – und beziehen Sie Zertifikate direkt aus Ihrer eigenen PKI.
  </p>
  <div class="mt-3 d-flex flex-wrap gap-2">
    <a href="https://glatzert.github.io/ACME-Server-ADCS/docs-v3.0/prereqs.html"
       class="btn btn-light">Quickstart-Anleitung</a>
    <a href="https://github.com/glatzert/ACME-Server-ADCS"
       class="btn btn-outline-light">GitHub</a>
  </div>
</div>

---

## Features auf einen Blick

<div class="row row-cols-1 row-cols-sm-2 row-cols-lg-3 g-3 my-2">

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🔒</span>
      <h3>RFC 8555 konform</h3>
      <p>Vollständig konformer ACME-Server – interoperabel mit jedem standardkonformen Client ohne Anpassungen.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🔌</span>
      <h3>Jeder ACME-Client</h3>
      <p>Certbot, win-acme, ACME-PS, acme.sh und viele weitere Clients funktionieren direkt out-of-the-box.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">✅</span>
      <h3>Mehrere Challenge-Typen</h3>
      <p>Unterstützt <code>http-01</code>, <code>dns-01</code> und <code>tls-alpn-01</code> sowie experimentelle Typen für spezielle Szenarien.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🌐</span>
      <h3>DNS- & IP-Zertifikate</h3>
      <p>Zertifikate für DNS-Namen und IP-Adressen (RFC 8738) – ideal für interne Dienste ohne öffentliche DNS-Einträge.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🔑</span>
      <h3>External Account Binding</h3>
      <p>EAB ermöglicht die Bindung von ACME-Accounts an vordefinierte Berechtigungen und Unternehmensrichtlinien.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">📋</span>
      <h3>Certificate Profiles</h3>
      <p>Unterschiedliche ADCS-Templates, CA-Server oder Laufzeiten je Anwendungsfall – flexibel konfigurierbar.</p>
    </div>
  </div>

</div>

---

## Challenge-Typen im Detail

<h3 class="features-section-title">Unterstützte Validierungsmethoden</h3>

Der ACME-ADCS-Server unterstützt folgende Challenge-Typen zur Domainvalidierung:

<ul class="badge-list">
  <li>http-01</li>
  <li>dns-01</li>
  <li>tls-alpn-01</li>
  <li class="experimental">dns-persist-01</li>
  <li class="experimental">device-attest-01</li>
</ul>

`http-01` und `dns-01` sind die am weitesten verbreiteten Typen und werden von
nahezu allen ACME-Clients unterstützt. `tls-alpn-01` erlaubt die Validierung
ausschließlich über TLS auf Port 443 gemäß [RFC 8737](https://datatracker.ietf.org/doc/rfc8737/)
und benötigt weder Port 80 noch einen DNS-Eintrag.

Die experimentellen Challenge-Typen befinden sich noch in der
Standardisierungsphase. `device-attest-01` ermöglicht die Ausstellung von
Client-Zertifikaten und wird aktuell von Apple-Geräten unterstützt.

---

## Identifier-Typen

<h3 class="features-section-title">Welche Identifiers werden unterstützt?</h3>

<ul class="badge-list">
  <li>dns (RFC 8555)</li>
  <li>ip (RFC 8738)</li>
  <li class="experimental">permanent-identifier</li>
  <li class="experimental">hardware-module</li>
</ul>

Neben klassischen DNS-Namen können auch **IP-Adressen** als Identifier in
Zertifikate aufgenommen werden – ein häufiger Bedarf in internen
Unternehmensnetzen, in denen Dienste nur per IP erreichbar sind.

---

## Certificate Profiles

<h3 class="features-section-title">Flexibles Profilsystem</h3>

Profile erlauben es, je nach Einsatzszenario unterschiedliche Konfigurationen
bereitzustellen:

- **Automatic** – Der Server wählt automatisch das passende Profil anhand des Identifiers aus.
- **Client-selected** – Der ACME-Client wählt aktiv ein Profil, konform zum [ACME-Profiles-Draft](https://datatracker.ietf.org/doc/draft-aaron-acme-profiles/01/).

So lassen sich beispielsweise für Webserver-Zertifikate ein anderes ADCS-Template
verwenden als für IoT-Geräte oder Client-Zertifikate – alles aus einer
zentralen Installation.

---

## Weitere Funktionen

- **CAA-Validierung** – Prüfung von Certification Authority Authorization Records und Method Binding gemäß [RFC 8657](https://datatracker.ietf.org/doc/rfc8657/).
- **ExternalAccountBinding (EAB)** – Accounts an Unternehmensrichtlinien binden; [Dokumentation](https://glatzert.github.io/ACME-Server-ADCS/docs/eab.html).
- **ADCS Auto-Enrollment** – Nutzt die vorhandene Auto-Enrollment-Konfiguration des ADCS-Templates.
- **Modernes .NET** – Basiert auf ASP.NET Core für eine wartbare und erweiterbare Architektur.
- **SBOM** – Enthält eine Software Bill of Materials (CycloneDX) für Transparenz und Compliance.

---

## Lizenz & Kosten

<h3 class="features-section-title">Wer darf die Software kostenfrei nutzen?</h3>

<table class="pricing-table">
  <thead>
    <tr>
      <th>Nutzergruppe</th>
      <th>Bedingung für kostenfreie Nutzung</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Privatpersonen</td>
      <td>Keine Gewinnerzielungsabsicht</td>
    </tr>
    <tr>
      <td>Bildungsanbieter</td>
      <td>Kursgebühren &lt; 500 EUR pro Semester</td>
    </tr>
    <tr>
      <td>Unternehmen</td>
      <td>Gesamtumsatz &lt; 10 Mio. EUR</td>
    </tr>
    <tr>
      <td>Alle</td>
      <td>Test- und Evaluierungszwecke</td>
    </tr>
  </tbody>
</table>

Für die kommerzielle Nutzung außerhalb dieser Grenzen beträgt die Lizenzgebühr
**1.500 EUR zzgl. MwSt.** mit unbegrenzter Laufzeit. Wartungs- und
Einrichtungsverträge können separat vereinbart werden.

Zum Erhalt eines Angebots wenden Sie sich an [thomas@th11s.de](mailto:thomas@th11s.de).

<div class="features-cta">
  <h2>Jetzt loslegen</h2>
  <p>Verbinden Sie Ihren ADCS in wenigen Schritten mit dem ACME-Protokoll.</p>
  <a href="https://glatzert.github.io/ACME-Server-ADCS/docs-v3.0/prereqs.html"
     class="btn btn-light">Dokumentation (V3.0)</a>
  <a href="https://github.com/glatzert/ACME-Server-ADCS"
     class="btn btn-outline-light">GitHub-Repository</a>
  <a href="mailto:thomas@th11s.de"
     class="btn btn-outline-light">Lizenz anfragen</a>
</div>
