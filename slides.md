# Cascade Presentation

--

## Was ist Cascade Persist & Remove

---

## Allgemeine Informationen

> Im Object-Relational Mapping (ORM)-Framework, gibt es die Konzepte des "Cascade Persist" und "Cascade Remove".
> Beschreiben das Verhalten beim Speichern und Löschen von Objekten in einer Datenbank

---

## Persist

> Cascade Persist" bezieht sich auf die automatische Speicherung von verknüpften Objekten, wenn das Hauptobjekt persistiert wird.

---

## Remove

> Wenn ein Hauptobjekt gelöscht wird, können Sie die Cascade-Entfernung konfigurieren, um sicherzustellen, dass die assoziierten Objekte ebenfalls entfernt werden, ohne dass Sie sie explizit löschen müssen.

--

## Vorteile & Nachteile

---


## Persist
Vorteile:
> Einfache und effiziente Speicherung
> Verbesserte Code-Lesbarkeit
> Vermeidung von Redundanz

Nachteile:
> Performanceauswirkungen
> Komplexität der Datenmanipulation

---

## Remove
 Vorteile:
> Datenintegrität
> Vereinfachte Datenlöschung

Nachteile:
> Unerwarteter Datenverlust
> Datenintegritätsprobleme
--

## Integration in Entity Cart.php






