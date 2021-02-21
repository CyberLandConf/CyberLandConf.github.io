---
layout: page
title: Late Night Enterprise Edition Bingo
permalink: /enterprise-bingo/
hidden: true
order: 99
---

![Bingo Logo](/assets/enterprise-bingo/bingo-header-big.png){:.image-max-height}


<div>
    <style>
    .grid-container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr 1fr 1fr;
    gap: 0px 0px;
    grid-template-areas:
        "cell-0-0 cell-0-1 cell-0-2 cell-0-3 cell-0-4"
        "cell-1-0 cell-1-1 cell-1-2 cell-1-3 cell-1-4"
        "cell-2-0 cell-2-1 cell-2-2 cell-2-3 cell-2-4"
        "cell-3-0 cell-3-1 cell-3-2 cell-3-3 cell-3-4"
        "cell-4-0 cell-4-1 cell-4-2 cell-4-3 cell-4-4";
    }
    .cell {
        border-style: solid;
        border-color: black;
        border-width: 2px;
        padding: 32px 32px 32px 32px;
        text-align: center;
        font-weight: bold;
    }
    .free-cell {
        background-color: green;
        font-size: 32px;
    }

    .cell-0-0 { grid-area: cell-0-0; }
    .cell-0-1 { grid-area: cell-0-1; }
    .cell-0-2 { grid-area: cell-0-2; }
    .cell-0-3 { grid-area: cell-0-3; }
    .cell-0-4 { grid-area: cell-0-4; }
    .cell-1-0 { grid-area: cell-1-0; }
    .cell-1-1 { grid-area: cell-1-1; }
    .cell-1-2 { grid-area: cell-1-2; }
    .cell-1-3 { grid-area: cell-1-3; }
    .cell-1-4 { grid-area: cell-1-4; }
    .cell-2-0 { grid-area: cell-2-0; }
    .cell-2-1 { grid-area: cell-2-1; }
    .cell-2-2 { grid-area: cell-2-2; }
    .cell-2-3 { grid-area: cell-2-3; }
    .cell-2-4 { grid-area: cell-2-4; }
    .cell-3-0 { grid-area: cell-3-0; }
    .cell-3-1 { grid-area: cell-3-1; }
    .cell-3-2 { grid-area: cell-3-2; }
    .cell-3-3 { grid-area: cell-3-3; }
    .cell-3-4 { grid-area: cell-3-4; }
    .cell-4-0 { grid-area: cell-4-0; }
    .cell-4-1 { grid-area: cell-4-1; }
    .cell-4-2 { grid-area: cell-4-2; }
    .cell-4-3 { grid-area: cell-4-3; }
    .cell-4-4 { grid-area: cell-4-4; }
    </style>


    <div class="grid-container">
        <div class="cell cell-0-0"></div>
        <div class="cell cell-0-1"></div>
        <div class="cell cell-0-2"></div>
        <div class="cell cell-0-3"></div>
        <div class="cell cell-0-4"></div>
        <div class="cell cell-1-0"></div>
        <div class="cell cell-1-1"></div>
        <div class="cell cell-1-2"></div>
        <div class="cell cell-1-3"></div>
        <div class="cell cell-1-4"></div>
        <div class="cell cell-2-0"></div>
        <div class="cell cell-2-1"></div>
        <div class="cell cell-2-2 free-cell">❤️</div>
        <div class="cell cell-2-3"></div>
        <div class="cell cell-2-4"></div>
        <div class="cell cell-3-0"></div>
        <div class="cell cell-3-1"></div>
        <div class="cell cell-3-2"></div>
        <div class="cell cell-3-3"></div>
        <div class="cell cell-3-4"></div>
        <div class="cell cell-4-0"></div>
        <div class="cell cell-4-1"></div>
        <div class="cell cell-4-2"></div>
        <div class="cell cell-4-3"></div>
        <div class="cell cell-4-4"></div>
    </div>

    <script type="text/javascript">

    var buzzwords = ["SOAP", "LAYER", "ARCHITEKTUR", "SOA", "AGIL", "B2B",
    "BIG DATA", "CLOUD", "CONTAINER", "CONTINUOUS DELIVERY", "CONTINUOUS INTEGRATION",
    "PATTERN", "DEVOPS", "AI", "LEAN", "FUNCTIONAL",
    "MICROSERVICE", "MODULARITY", "MONOLITH", "SERVERLESS", "BLOCKING",
    "NON-BLOCKING", "SQL", "NOSQL", "REST", "REACTIVESCRUM",
    "TDD", "UML", "AWS", "STATELESS", "STREAMING",
    "AGILE", "WEBSERVICE", "SAML", "JWT", "KEYCLOAK",
    "APPLICATION SERVER", "SPECIFICATION", "3 LAYER", "EJB", "JPA",
    "JMS", "JDBC", "KAFKA", "SPRING BOOT", "ACTIVE MQ",
    "LDAP", "CERTIFIED", "XA TRANSACTION", "2 FACE COMMIT", "ROLLBACK",
    "TOMCAT", "JAKARTAEE", "JAVA-EE", "J2EE", "MQ-SERIES",
    "WEBSPHERE", "WEBLOGIC", "JBOSS"];


    function getRandomInt(max) {
    return Math.floor(Math.random() * Math.floor(max));
    }

    function setText(divSelector, value) {
        document.querySelector(divSelector).innerHTML = value;
    }
    
    function createBingo() {
        var usedBuzzwords = [];
        while(usedBuzzwords.length <= 24) {
            var selectedWord = buzzwords[getRandomInt(buzzwords.length)];
            while(usedBuzzwords.includes(selectedWord)) {
                selectedWord = buzzwords[getRandomInt(buzzwords.length)];
            }
            usedBuzzwords.push(selectedWord);
        }
        setText('.cell-0-0', usedBuzzwords[0]);
        setText('.cell-0-1', usedBuzzwords[1]);
        setText('.cell-0-2', usedBuzzwords[2]);
        setText('.cell-0-3', usedBuzzwords[3]);
        setText('.cell-0-4', usedBuzzwords[4]);
        setText('.cell-1-0', usedBuzzwords[5]);
        setText('.cell-1-1', usedBuzzwords[6]);
        setText('.cell-1-2', usedBuzzwords[7]);
        setText('.cell-1-3', usedBuzzwords[8]);
        setText('.cell-1-4', usedBuzzwords[9]);
        setText('.cell-2-0', usedBuzzwords[10]);
        setText('.cell-2-1', usedBuzzwords[11]);

        setText('.cell-2-3', usedBuzzwords[12]);
        setText('.cell-2-4', usedBuzzwords[13]);
        setText('.cell-3-0', usedBuzzwords[14]);
        setText('.cell-3-1', usedBuzzwords[15]);
        setText('.cell-3-2', usedBuzzwords[16]);
        setText('.cell-3-3', usedBuzzwords[17]);
        setText('.cell-3-4', usedBuzzwords[18]);
        setText('.cell-4-0', usedBuzzwords[19]);
        setText('.cell-4-1', usedBuzzwords[20]);
        setText('.cell-4-2', usedBuzzwords[21]);
        setText('.cell-4-3', usedBuzzwords[22]);
        setText('.cell-4-4', usedBuzzwords[23]);
    }
    document.onload = createBingo();
    </script>

</div>