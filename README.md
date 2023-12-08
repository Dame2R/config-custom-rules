# Dynamische Policies
**Schritt-für-Schritt Anleitung**

1.  **Installation des AWS Config RDK**

`pip install rdk`

2.  **Erstellen einer Custom Rule**

-  Für periodische Prüfung: `rdk create RULE_NAME --maximum-frequency TwentyFour_Hours`
-  Für spezifische Ressourcentypen: `rdk create RULE_NAME --resource-types RESOURCE_TYPE`

3.  **Regellogik implementieren**

**Bearbeiten der rule_name.py Datei mit der gewünschten Logik, in beliebiger Programmiersprache und IDE.**

4.  **Deployment der Regel**

`rdk deploy RULE_NAME`

5.  **Konfiguration in AWS Config**

**Automatische Anlage der Lambda Funktion, IAM-Rolle, Config Rule und CloudWatch Protokollgruppe.**
