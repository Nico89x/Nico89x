# Nico Joschke

**Junior Workflow Automation · n8n, REST-APIs und Prozessintegration**

Ich suche den Einstieg in die Workflow-Automatisierung und API-Integration. Meine Arbeitsproben zeigen, wie ich Geschäftsprozesse in nachvollziehbare Abläufe übersetze und dabei Eingaben, Dubletten, Fehlerfälle und Freigaben berücksichtige.

[Portfolio ansehen](https://nico89x.github.io/nico-joschke-automation-portfolio/) · [Kurzprofil](https://nico89x.github.io/nico-joschke-automation-portfolio/kurzprofil.html)

## Arbeitsproben zur Automatisierung

### [Operations Hub](https://github.com/Nico89x/nico-joschke-automation-portfolio/tree/main/projects/multi-agent-ai-operations-hub)

Ein n8n-Workflow nimmt Automatisierungsanfragen per Webhook entgegen, prüft Eingaben und Dubletten und speichert in PostgreSQL einen Entwurf mit Audit-Log zur menschlichen Freigabe.

**Mein Beitrag.** Ich habe die Anforderungen an die Freigabe und die Grenzen für externe Aktionen festgelegt. Dazu gehört, dass eine wiederholte Freigabe mit HTTP 409 abgewiesen wird und der freigegebene Entwurf lokal bleibt.

**Prüfbeispiel.** Der End-to-End-Test schickt dieselbe Anfrage zweimal und prüft, dass beide Aufrufe auf denselben Datensatz verweisen. Er prüft außerdem, dass eine wiederholte Freigabe keinen zweiten Audit-Eintrag erzeugt. [Testskript](https://github.com/Nico89x/nico-joschke-automation-portfolio/blob/main/projects/multi-agent-ai-operations-hub/scripts/verify-clean-e2e.mjs) · [GitHub-Actions-Lauf](https://github.com/Nico89x/nico-joschke-automation-portfolio/actions/runs/36835141067) · [Demo-Anleitung](https://github.com/Nico89x/nico-joschke-automation-portfolio/blob/main/projects/multi-agent-ai-operations-hub/docs/DEMO_RUNBOOK.md)

### [Lead-to-Offer](https://github.com/Nico89x/nico-joschke-automation-portfolio/tree/main/projects/lead-to-offer)

Drei n8n-Workflows bilden den Eingang einer Kundenanfrage, die Aufbereitung von CRM-Daten und die Erstellung eines internen Angebotsentwurfs ab. Das gemeinsame Datenmodell ist für Notion vorgesehen.

**Mein Beitrag.** Ich habe den fachlichen Ablauf und die Anforderungen an Lead- und Angebotsdaten definiert. Dazu gehören Pflichtfelder beim Eingang und klare Regeln für die Berechnung von Angebotssummen.

**Prüfbeispiel.** Die Regressionstests prüfen unter anderem, dass gültige Leads normalisiert und doppelte Leistungspakete nicht zweimal berechnet werden. Die Tests führen den exportierten JavaScript-Code mit synthetischen Daten aus. Der vollständige Durchlauf mit Notion bleibt offen. [Workflow-Exporte und Testanleitung](https://github.com/Nico89x/nico-joschke-automation-portfolio/tree/main/projects/lead-to-offer) · [Regressionstests](https://github.com/Nico89x/nico-joschke-automation-portfolio/blob/main/test/portfolio-site.test.mjs)

## Weitere Arbeitsproben

| Projekt | Was sich prüfen lässt |
| --- | --- |
| [ReleaseWatch](https://github.com/Nico89x/nico-joschke-automation-portfolio/tree/main/projects/release-support-triage) | Ein Node.js-Adapter liest öffentliche GitHub-Release-Daten. Tests decken ungültige Antworten, Timeouts und Rate-Limits ab. |
| [Grocery Store](https://github.com/Nico89x/ai-grocery-store-automation) | Eine React-/TypeScript-Demo und ein separates Node.js-/SQLite-Backend zeigen Bestellverarbeitung und Wiederholung ohne doppelte Buchung. Ein erfolgreicher n8n-Testempfang ist [dokumentiert](https://github.com/Nico89x/ai-grocery-store-automation/blob/main/automation/README.md). [Browserdemo](https://nico89x.github.io/ai-grocery-store-automation/#/simulation) |
| [CyberGuard AI](https://github.com/Nico89x/CyberGuard-AI) | Lokaler Python-/FastAPI-Prototyp mit validierten Testereignissen, authentifiziertem Dashboard und automatisierten API-Tests. [Windows-CI-Lauf](https://github.com/Nico89x/CyberGuard-AI/actions/runs/41647379655) |
| [FIMAG](https://github.com/Nico89x/fimag-landingpage) | Statisches Website-Gestaltungskonzept mit responsiver Oberfläche und clientseitiger Formularvalidierung. |

**Technik im Portfolio:** n8n, Webhooks, REST, JSON, JavaScript/TypeScript, Node.js, PostgreSQL und SQLite. Ergänzende Arbeitsproben zeigen Python/FastAPI, React, Vitest, pytest, Playwright und GitHub Actions.

## Arbeitsweise und Verfügbarkeit

Ich verantworte Konzept, fachliche Anforderungen und die Bewertung der Prüfergebnisse. Bei Implementierung, Dokumentation und technischen Prüfungen habe ich KI-Unterstützung genutzt. Die Arbeitsproben dokumentieren Portfolio- und Testsysteme mit synthetischen Geschäftsdaten.

Ich suche eine Junior-Rolle mit fachlichem Austausch und strukturierter Einarbeitung, in **Vollzeit oder Teilzeit und vollständig remote innerhalb Deutschlands**.
