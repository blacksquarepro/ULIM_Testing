**Question 1:** Descrieti cheltuielile indirecte, repartizarea cheltuielilor pe nivelele testarii, repartizarea cheltuielilor pe fazele procesului de testare si caile de reducere a cheltuielilor de testare.<br>

**Answer 1:**
Cheltuielile in procesul testarii includ:
* cheltuieli pentru planificare a procesului de testare
* cheltuieli pentru prepararea testelor
* cheltuieli pentru realizarea testelor
* cheltuieli pentru analiza si raportarea rezultatelor testelor

Din costuri indirecte in procesul de testare software evedentiaza urmatoarele tipuri de costuri:
* costuri asociate cu rescrierea software
* costuri asociate cu restabilirea lucrului programelor
* costuri pentru actiuni corective
* costuri provocate de testare incalitativa (costul daunelor)
* costuri pentru sedinte si analiza
* costuri pentru debugging al software si identificarea/documentarea greselilor
* costuri asociate cu necesitatea testarii repetitive al software

Ca metode de reducere a costurilor de testare pot fi considerate urmatoarele masuri:
1. Documentarea cerintelor cit mai detaliata si completa la etapa analizei business
2. Implementarea procesului de versionare a codului sursa al solutiei si backup al datelor
3. Implementarea testelor automatizate la toate etapele dezvoltarii in lant, incepand cu unit testing si finisand cu E2E testare
4. Automatizarea extensiva a testarii cu scopul reducerii cheltuielele pentru resurse umane (testing manual)
5. Insertarea testelor in pipe-urile Continuous Integration (CI) cu scopul identificarii erorilor in regim automat la build-ul solutiei
6. Implementarea pipe-urilor CI/CD multi-environment cu scopul testarii extensive al solutiilor in regim automat si identificarii erorilor pe multiple medii (DEV/TEST/STAGING/PROD) pana livrarea produsului software in mediul PROD

---

**Question 2:** Explicati testarea automata, tipurile de testare automata, limitele testarii automate si tipurile de unelte pentru testarea automata.<br>
**Answer 2:**

Testarea automata - tip de testare al produselor software, in care testarea este executata de catre instrumente automatice, implementand unul sau mai multe scenarii programate de testatori.

Evedentiaza urmatoarele tipuri de testare automata:
* Static Code Analysis - analizarea codului sursa in vederea conventiilor limbajului, linting-ului, stilului de cod, securitatii codului si potentialilor probleme
* Unit Testing - testarea metodelor al codului sursa al solutiilor
* Integration Testing - testarea integrationala intre componente al solutiei sau intre sisteme (ex. API si schimb de date)
* Performance/Load/Stress Testing - testarea performantei solutiei informationale prin simularea incarcarii acestei din partea utilizatorilor
* Security/Penetration Testing - testarea securitatii solutiei informationale si protectiei ei contra atacurilor
* UI Testing - testarea interfatei solutiei si corespunderii al nivelului UI cerintelor formate pentru diferite platforme si device-uri
* E2E Testing - testarea automatizata a solutiei din perspectiva utilizatorilor prin simularea scenariilor de utilizare programate de catre testatori in baza test case-urilor

Din instrumente de testare automata pentru fiecare tip de testare automata definesc urmatoarele cele mai populare:
* Static Code Analysis - SonarQube, CodeClimate, PVS Studio
* Unit Testing - in depentinta de limbaj de programare, ex. Python - UnitTest (librarie standarta)
* Integration Testing - in dependenta de limbaj/framework, ex. Python - PyTest, Robot
* Performance/Load/Stress Testing - JMeter, K6.io
* Security/Penetration Testing - OWASP Top-10 scanner, Kali Linux application suite
* UI Testing - Selenium, Telerik, Cucumber
* E2E Testing - Cypress, Selenium, CodeceptJS, TestCaffe
