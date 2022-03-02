## Konformitätserklärung [(CapabilityStatement)](http://hl7.org/fhir/capabilitystatement.html)

Jede Instanz eines bestätigungsrelevanten Systems MUSS an ihrem Endpunkt eine [CapabilityStatement](http://hl7.org/fhir/capabilitystatement.html)-Ressource bereitstellen.

Hierzu MUSS die [capabilities-Interaktion gemäß FHIR-Spezifikation](http://hl7.org/fhir/http.html#capabilities) unterstützt werden.
Der MODE-Parameter kann ignoriert werden.

Das CapabilityStatement in dieser Spezifikation stellt die Anforderungen seitens der gematik dar. (`kind` = "requirements"). Zur Unterscheidung von Anforderungen, die erfüllt werden MÜSSEN gegenüber jenen, die erfüllt werden KÖNNEN, wird die [CapabilityStatement-Expectation](http://hl7.org/fhir/extension-capabilitystatement-expectation.html)-Extension mit den möglichen Werten "SHALL" (=MUSS) und "MAY" (=KANN) verwendet.

Eine Server-Instanz MUSS ihrerseits ein CapabilityStatement vom `kind`= "instance" liefern und im Element `software` den Namen und die Versionsnummer angeben.

Das CapabilityStatement der Instanz MUSS alle Funktionalitäten auflisten, die im folgenden CapabilityStatement mit "SHALL" gekennzeichnet sind. Das CapabilityStatement KANN darüber hinaus die mit "MAY" gekennzeichneten Funktionalitäten, sowie weitere Funktionalitäten auflisten, sofern diese in der Instanz implementiert wurden.

Die Verwendung der [CapabilityStatement-Expectation](http://hl7.org/fhir/extension-capabilitystatement-expectation.html)-Extension ist im CapabilityStatement der Server-Instanz nicht erforderlich.

## CapabilityStatement (Requirement) ISiK-Medikation

Die Bereitstellung des CapabilityStatments für das Modul "Medikation" erfolgt zusammen mit der Festlegung der bestätigungsrelevanten Systeme in Stufe 2

Für Systeme, die das Modul "Medikation" implementieren, ist außerdem die Erfüllung der Mindestanforderungen des [Moduls "Basis"](https://simplifier.net/guide/ImplementierungsleitfadenISiK-Basismodul/Einfuehrung) erforderlich:

Canonical: https://gematik.de/fhir/ISiK/v2/CapabilityStatement/core-server

[Link Simplifier Profil Übersicht](https://simplifier.net/isik/isik-capabilitystatement-medikation-server)

{{render:https://gematik.de/fhir/ISiK/v2/CapabilityStatement/medikation-server}}

