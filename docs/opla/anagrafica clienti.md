# Anagrafica clienti

nome applicativo: o_cli2_g

link interno [Elenco clienti](#elenco-clienti)

link altro file 
[procedura](../../procedure/Procedura disposizione campione stampa/#procedura)

## Voci menu

### Anagrafica

!!! tip inline end "Nota a destra"

    Nota sulla manutenzione
	dei clienti 
	
manutenzione dei clienti (1) 
{ .annotate }

1.  :man_raising_hand: nota su anagrafica clienti: con `codice`, __testo
    bold__, ... tutto in markdown.

- lista
- secondo
- terzo

* primo
* secondo
* terzo


### Elenco clienti

=== "Lista senza ordine"

    * Sed sagittis eleifend rutrum
    * Donec vitae suscipit est
    * Nulla tempor lobortis orci

=== "Lista ordinata"

    1. Sed sagittis eleifend rutrum
    2. Donec vitae suscipit est
    3. Nulla tempor lobortis orci


!!! note "Nota aperta"

    nota di prova  
    aperta

??? note "Personalizzazione clienti"

    nota di __prova__
	
	??? abstract "Cliente 1"
	
		nota del cliente 1
		
	??? abstract "Cliente 2"
	
		nota del cliente 2
		
### Elenco due

| Voce menu   | Description                          |
| ----------- | ------------------------------------ |
| voce a      | esempio 1  |
| voce b      |   |
| voce c      | con icona :material-close:|

``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```

``` mermaid
sequenceDiagram
  autonumber
  Alice->>John: Hello John, how are you?
  loop Healthcheck
      John->>John: Fight against hypochondria
  end
  Note right of John: Rational thoughts!
  John-->>Alice: Great!
  John->>Bob: How about you?
  Bob-->>John: Jolly good!
```

``` mermaid
stateDiagram-v2
  state fork_state <<fork>>
    [*] --> fork_state
    fork_state --> State2
    fork_state --> State3

    state join_state <<join>>
    State2 --> join_state
    State3 --> join_state
    join_state --> State4
    State4 --> [*]
```

``` mermaid
classDiagram
  Person <|-- Student
  Person <|-- Professor
  Person : +String name
  Person : +String phoneNumber
  Person : +String emailAddress
  Person: +purchaseParkingPass()
  Address "1" <-- "0..1" Person:lives at
  class Student{
    +int studentNumber
    +int averageMark
    +isEligibleToEnrol()
    +getSeminarsTaken()
  }
  class Professor{
    +int salary
  }
  class Address{
    +String street
    +String city
    +String state
    +int postalCode
    +String country
    -validate()
    +outputAsLabel()  
  }
```

``` mermaid
erDiagram
  CUSTOMER ||--o{ ORDER : places
  ORDER ||--|{ LINE-ITEM : contains
  LINE-ITEM {
    string name
    int pricePerUnit
  }
  CUSTOMER }|..|{ DELIVERY-ADDRESS : uses
```

``` mermaid
---
config:
  kanban:
    ticketBaseUrl: 'http://62.110.6.89:61221/view.php?id=#TICKET#'
---
kanban
  Todo
    [Create Documentation]
    docs[Create Blog about the new diagram]
  [In progress]
    id6[Create renderer so that it works in all cases. We also add som extra text here for testing purposes. And some more just for the extra flare.]
  id9[Ready for deploy]
    id8[Design grammar]@{ assigned: 'knsv' }
  id10[Ready for test]
    id4[Create parsing tests]@{ ticket: 8000, assigned: 'K.Sveidqvist', priority: 'High' }
    id66[last item]@{ priority: 'Very Low', assigned: 'knsv' }
  id11[Done]
    id5[define getData]
    id2[Title of diagram is more than 100 chars when user duplicates diagram with 100 char]@{ ticket: 7900, priority: 'Very High'}
    id3[Update DB function]@{ ticket: 8003, assigned: knsv, priority: 'High' }

  id12[Can't reproduce]
    id3[Weird flickering in Firefox]
```

- ==This was marked (highlight)==
- ^^This was inserted (underline)^^ Testo normale e __testo Bold__
- ~~This was deleted (strikethrough)~~


++ctrl+alt+del++

Si usano icone con nome :material-truck: oppure :octicons-mail-24: o emoticons :smile:
[ricerca codici icone](https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/ "Ricerca di codici icone o emoticons")

#### markdown
ogni riga di testo
si compatta a meno che non finisce con sue spazi prima  
dell'enter

>testo quotato che continua
fino alla fine
>> e può essere indentato  

>e tornare normale

****

testo sotto riga orizzontale


#### card grid

<div class="grid cards" markdown>

-   :material-clock-fast:{ .lg .middle } __Set up in 5 minutes__

    ---

    Install [`mkdocs-material`](#) with [`pip`](#) and get up
    and running in minutes

    [:octicons-arrow-right-24: Getting started](#)

-   :fontawesome-brands-markdown:{ .lg .middle } __It's just Markdown__

    ---

    Focus on your content and generate a responsive and searchable static site

    [:octicons-arrow-right-24: Reference](#)

-   :material-format-font:{ .lg .middle } __Made to measure__

    ---

    Change the colors, fonts, language, icons, logo and more with a few lines

    [:octicons-arrow-right-24: Customization](#)

-   :material-scale-balance:{ .lg .middle } __Open Source, MIT__

    ---

    Material for MkDocs is licensed under MIT and available on [GitHub]

    [:octicons-arrow-right-24: License](#)

</div>

