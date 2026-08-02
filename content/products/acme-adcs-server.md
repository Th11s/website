+++
title = "ACME ADCS Server: Automatisierung für Ihre Zertifikate"
subtitle = "ACME-Protokoll für Ihre Windows-PKI"
summary = "Ein RFC 8555 kompatibler Server mit ADCS als Backend."
description = "Automatisierte Zertifikatsausstellung für Ihre ADCS Umgebung. Sicher, zuverlässig und ohne manuellen Aufwand. Einfache Implementierung. Produkt kostenfrei testen."
icon = "🔐"
weight = 1
+++

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

## Manuelle Zertifikate? Nicht mehr.

Zertifikate laufen ab, werden übersehen oder falsch ausgestellt — und genau dann wird es teuer.
Manuelle Prozesse kosten Zeit, erzeugen Fehler und erhöhen das Sicherheitsrisiko.

ACME ADCS Server automatisiert Ausstellung und Erneuerung vollständig über das ACME-Protokoll.
Er verbindet die Microsoft Active-Directory Certificate Authority mit dem Automatic Certificate
Management Environment (bekannt von Let's Encrypt) und ermöglicht Ihnen, mit einem ACME
(RFC 8555) kompatiblen Client Zertifikate Ihrer eigenen PKI auszustellen —
so behalten Sie jederzeit Kontrolle und Sicherheit, ohne zusätzlichen Aufwand.

---

## Warum ACME-ADCS Server überzeugt

<div class="row row-cols-1 row-cols-sm-2 g-3 my-2">

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🧪</span>
      <h3>Kostenfrei testen</h3>
      <p>ACME ADCS kann vollständig erprobt werden, bevor eine Entscheidung fällt. Keine Risiken, keine Verpflichtungen.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">👁️</span>
      <h3>Offener Quellcode</h3>
      <p>Die gesamte Lösung ist transparent einsehbar. Sicherheitsprüfungen, Audits und interne Reviews sind problemlos möglich.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🔗</span>
      <h3>Nahtlose Integration</h3>
      <p>Direkte Einbindung in bestehende Infrastrukturen — ideal für Unternehmen mit individuellen Prozessen oder Compliance-Anforderungen.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">🛠️</span>
      <h3>Anpassbar</h3>
      <p>Durch den offenen Quellcode kann die Lösung erweitert, integriert oder modifiziert werden, um perfekt zu internen Abläufen zu passen.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">💶</span>
      <h3>Moderate Lizenzkosten</h3>
      <p>1.500 € einmalig pro Unternehmensgruppe — kein Extra-Preis pro Instanz, Benutzer, Server oder Zertifikat.</p>
    </div>
  </div>

  <div class="col">
    <div class="feature-card">
      <span class="feature-icon">⭐</span>
      <h3>Bewährt & aktiv</h3>
      <p>Über 170 Stars auf GitHub, viele zufriedene Kunden weltweit und aktive Weiterentwicklung.</p>
    </div>
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

## Installation

Die Installation von ACME ADCS ist bewusst einfach gehalten.
Alles, was Sie benötigen, finden Sie direkt auf GitHub.

1. Öffnen Sie das offizielle [ACME ADCS GitHub-Repository](https://github.com/glatzert/ACME-Server-ADCS).
2. Folgen Sie der dort beschriebenen Installationsanleitung Schritt für Schritt.
3. Passen Sie die Konfiguration an Ihre bestehende ADCS-Umgebung an.
4. Starten Sie den Web-Server – fertig.

Die Dokumentation enthält alle Details zu Setup, Konfiguration, Systemvoraussetzungen und
Best Practices. Sie können ACME ADCS sofort testen und eine Lizenz erst erwerben, wenn Sie
es produktiv einsetzen möchten.

<a href="https://glatzert.github.io/ACME-Server-ADCS/docs-v3.0/prereqs.html" class="btn btn-primary">Zur Dokumentation (V3.0)</a>

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

---

## Freiwillige Unterstützung

Wenn ACME ADCS Ihnen Zeit spart und graue Haare verhindert, dürfen Sie mir gern einen Kaffee
spendieren. Kein Muss — aber Koffein hält die Weiterentwicklung am Laufen:
[Thomas auf PayPal](https://paypal.me/TGlatzer) ☕
