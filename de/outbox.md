# Der Postausgang

**Postfach-Symbol → "Postausgang"**. Nichts geht raus, bis du es freigibst.

Jede E-Mail, jeder Beitrag oder jede Nachricht, die Taibu vorbereitet, landet hier als Entwurf. Die gelbe Zahl in der Leiste zeigt dir, wie viele warten.

## Prüfen

Im rechten Bereich siehst du, welche Routine oder welcher Skill den Entwurf erstellt hat, den Empfänger und den Inhalt. Den Inhalt kannst du erst direkt ändern, wenn du sagst, wie du ihn ändern willst. So weißt du immer, was du gerade tust:

- **Selbst bearbeiten** setzt den Cursor in den Text. Ändere, was du willst, dann **Änderungen speichern**. Bis du speicherst, ist der Entwurf mit "Bearbeitet, noch nicht gespeichert" markiert, und **Änderungen verwerfen** setzt ihn zurück.
- **Mit Agent bearbeiten** übergibt den Entwurf an einen Agenten für eine komplette Neufassung.

![Ein Entwurf wartet auf Freigabe](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/de/19-outbox.png)

| Schaltfläche | Was sie macht |
|---|---|
| **Freigeben und senden** | Markiert den Entwurf als freigegeben und stellt ihn dann zu |
| **Selbst bearbeiten** | Macht den Text bearbeitbar. **Änderungen speichern** schreibt ihn zurück |
| **Mit Agent bearbeiten** | Öffnet den Entwurf in einem Agenten für eine komplette Neufassung |
| **Überspringen** | Bringt dich zum nächsten Entwurf. Damit lehnst du diesen nicht ab. Er bleibt wartend |
| **In den Papierkorb** | Verwirft den Entwurf, mit einer Rückgängig-Option |

## Was "gesendet" bedeutet

Manche Verbindungen können nur einen Entwurf erstellen, aber nicht senden. Der Gmail-Konto-Connector ist das häufigste Beispiel: Er kann die Nachricht in deinen Gmail-Entwürfe-Ordner legen, aber nicht senden.

Taibu ist angewiesen, nie zu behaupten, etwas gesendet zu haben, wenn es nur einen Entwurf erstellt hat. Prüfe beim ersten Mal deinen Ordner für gesendete Nachrichten, wenn du einen neuen Kanal nutzt. Dann weißt du, welches Verhalten du bekommst.

## Warum du ihm vertrauen kannst

Die Regel wird an drei Stellen durchgesetzt: Routinen dürfen nicht senden, die App statt der KI verwaltet den Freigabe-Status, und die App spricht nie selbst mit externen Diensten. Die KI kann nicht in deinem Namen freigeben.
