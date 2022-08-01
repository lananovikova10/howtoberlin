# The sequence of steps

```mermaid
graph TB
    subgraph Before moving
        VISA --> P[Post a scan of your visa<br/>to YouTrack issue]
        VISA[Get National Visa D] --> BUY[Ask to book tickets]
        BUY --> TR[Travel to Germany]
        BOOK[Find a temporary accomodation, or<br/>ask the  Relocation manager<br/>to book accomodation for you] --> TR
        ST[Prepare your stuff<br/>to be moved by PrimeMovers]

        ST --> CAL[Inform PrimeMovers in 2-3 weeks<br/>about your things and when you are leaving]
    end
    TR --> SIM[Buy a German sim card. At first, prepaid is recommended, not contract. <br/>Best coverage in Berlin is at Telekom.de and its virtual operators<br/>Coverage of O2 Telefonica is worst, and Vodafone is in between<br/>See more info on the topic <a href='https://tinyurl.com/2p94c3sb'>in this article</a>]
    TR --> ACC[Arrive into temporary accomodation]
    TR --> SCH1[Get Schufa Auskunft<br/>without IBAN<br/>to JB office address<br/>via ImmobilienScout24.de,<br/>see description below]
    ACC --> WOH[Ask a landlord for Wohnungsgeber-Bestätigung]
    WOH --> |You need to register within 14 days after arrival.| REG[Register temporary residential address at Bürgeramt, aka Anmeldung.<br/>In case you're married -> whole family comes together<br/>with marriage and birth certificates for kids]
    REG --> MAIL[Put your surname on a mailbox, a frontdoor</br>and an apartment doorbell]
    MAIL --> TAX[Finanzamt generates<br/>Steuer-ID/Tax-ID<br/>for you in 3 days<br/>and sends it via<br/>papermail in 2 weeks.<br/>You can get it faster<br/>by coming to your<br/>Finanzamt in person]
    MAIL --> PAYSLIPS[Receive login<br/>and password<br/>for payslips by<br/>separate<br/>papermails]
    MAIL --> SSN[Receive<br/>social<br/>insurance<br/>number,<br/>inform HR]
    TAX --> STKL[In case you're married-><br/>come together to Finanzamt<br/>and explicitly tell them,<br/>which tax classes you've chosen.<br/>They will issue you two documents<br/>with your tax classes and tax ids]
    REG --> BANK[Open bank account<br/>at Sparkasse, DB, Commerz,<br/>or other, incl. neobanks]
    BANK --> IBAN[Get IBAN `International Bank Account Number`]
    IBAN & MAIL --> CARD[Receive bank card<br/>and its pincode with <br/>separate papermails]
    TAX & STKL --> HR1[Send scan of Tax ID and Tax Class to HR]
    REG & IBAN --> SCH2[Get Schufa Auskunft<br/>with IBAN and real address<br/>see description below]
    ACC -.-> MSFE[Ask landlord for<br/>`Mietschuldenfreiheitserklärung<br/>des Vorvermieters`]
    SCH1 & SCH2 -.-> PERM[Sign a contract for permanent accomodation,<br/>the best case: unlimited]
    IBAN --> PERM
    MSFE -.-> |Usually, new landlord wants to know,<br/>whether you don't have any debts to previous landlord|PERM
    PERM & CAL --> I[Inform PrimeMovers<br/>to deliver your stuff]
    PERM --> WOH2[Ask a landlord for Wohnungsgeber-Bestätigung]
    WOH2 --> REG2[Register your permanent<br/>address at town hall]
    REG2 --> INF[Inform companies about your address change,<br/>see their approx. list after the diagram]
    REG2 ----> AMEL[Apply for long-term work<br/>permit in Ausländerbehörde.<br/>Birgit recommends not earlier than<br/> 2-3 month after arrival.]
    PERM --> MAIL2[Put your surname on <br/>a mailbox,<br/>a frontdoor</br> and doorbell]
    MAIL2 --> INF
    AGB[Ask Birgit to issue<br/>Arbeitgeberbescheinigung] --> AMEL
    AMEL --> VNZH[Get work and residence long-permit.<br/>It can be a bluecard, or work visa]
    VNZH --> HR2[Send scan to HR]
    VNZH --> KINDERGELD[Apply for<br/>state benefits<br/>for children,<br/>if applicable,<br/>200eur/child]
    VNZH --> ELTERNGELD[Apply for<br/>state benefits<br/>for parents,<br/>if applicable,<br/>for child <1 y.o.]
```

Some more information on each step:
- [Anmeldung](anmeldung.md)
- [Tax ID](finanzamt.md)
- [Schufa Auskunft](schufa.md): credit history document.
Almost always it's required for an apartment viewing, and it's part of document list when applying for a contract.
At ImmobilienScout24.de, Schufa Auskunft can be ordered either for 29 Eur, or for free via paid ImmobilienScout24.de subscription.
Anyway ImmobilienScout24.de paid subscription for a couple of months is really required for non-zero chances to get good permanent apartment.
- `Inform companies about your address change`: JetBrains HR, insurance companies(health + others), banks, energy providers,
mobile operators, internet operator, insurance companies, car sharings, ImmoScout24.
Highly recommended: set up papermail redirects at [Deutsche Post](https://shop.deutschepost.de/shop/nachsenden-lagern/nachsendeservice.jsp?cid=DP_101002152)
and [PIN Mail](https://www.pin-ag.de/privatkunden/formulare/nachsendeauftrag).

After long-term residence, there will be the following ways to get permanent residence:
```mermaid
graph TB
        BC[In case you got Bluecard] -.-> B1[Pass German Language B1 exam]
        BC -.-> A1[Pass German language A1 exam]
        A1 --> |After 33 months from getting Bluecard|PMZHAPP[Apply for permanent residence]
        B1 --> |After 21 months from getting Bluecard|PMZHAPP

        WV[In case you got work visa] --> B1_wv[Pass German Language B1 exam]
        B1_wv --> |5 years of paying to pension fund|PMZHAPP
        PMZHAPP --> PMZH[Obtain permanent residence]
        PMZH -.-> MORT[Now you can freely apply for a mortgage<br/>Note: in _very_ rare cases, you can get mortgage<br/>without permanent residence]
```
