# Cascade Presentation

--

## Was ist Cascade Persist & Remove

---

## Allgemeine Informationen

> Im Object-Relational Mapping (ORM)-Framework, gibt es die Konzepte des "Cascade Persist" und "Cascade Remove".
> Sie Beschreiben das Verhalten beim Speichern und Löschen von Objekten in einer Datenbank

---

## Persist

> "Cascade Persist" bezieht sich auf die automatische Speicherung von verknüpften Objekten, wenn das Hauptobjekt persistiert wird.

---

## Remove

> Wenn ein Hauptobjekt gelöscht wird, kann man Cascade konfigurieren, um verknüpfte Objekte ebenfalls zu entfernen, ohne dass man sie explizit löschen muss.

--

## Vorteile & Nachteile

---


## Persist
Vorteile:
> Einfache und effiziente Speicherung.

> Verbesserte Code-Lesbarkeit.

> Zeitersparnis

Nachteile:
> Performanceauswirkungen.

> Komplexität der Datenmanipulation.

---

## Remove
 Vorteile:
> Datenintegrität.

> Vereinfachte Datenlöschung.

Nachteile:
> Unerwarteter Datenverlust.

> Datenintegritätsprobleme.
--

## Integration in Php


Integration in Entity Cart.php:
> #[ORM\OneToMany (mappedy: 'cart', targetEntity: CartProduct::class, cascade: ["persist", "remove"], orphanremoval: true)]

Integration in Enitity CartProduct.php: 
> #[ORM\ManyToOne (inversedBy: 'cartProducts") ]
#[ORM\ JoinColumn (nullable: false, onDelete: 'CASCADE") ]
private ?Product $product = nUll;
#[ORM\Column]
private ?int Samount = null;
#[ORM\ ManyToOne (inversedBy: 'cartProducts') ]
#[ORM\ JoinColumn (nullable: false, onDelete:
'CASCADE') ]
private ?Cart $cart = null;







