# The sequence of steps

```mermaid
graph TB
    subgraph Before moving
        VISA --> P[Post a scan of your visa to YouTrack issue]
        VISA[Get National Visa D] --> BUY[Ask to book tickets]
        BUY --> TR[Travel to Germany]
        TEMP[Find a temporary accomodation] --> TR
        TEMP --> BOOK[Ask the  Relocation manager to book accomodation for you]
        ST[Prepare your stuff to be moved by PrimeMovers]

        ST --> CAL[Inform PrimeMovers in 2-3 weeks about your things and when you are leaving]
    end
    BOOK --> TR
    TR --> SIM[Buy a German sim card. At first, prepaid is recommended, not contract. <br/>Best coverage in Berlin is at Telekom.de and its virtual operators like Lebara <br/>https://second.wiki/wiki/liste_der_mobilfunkprovider_in_deutschland.<br/>Coverage of O2 Telefonica is worst, and Vodafone is in between]
    SIM --> ACC[Get Temporary accomodation]
    ACC --> WOH[Ask a landlord for Wohnungsgeber-Bestätigung]
    WOH --> |You need to register within 14 days after arrival.| REG[Register temporary residential address at town hall aka Anmeldung. In case you're married -> whole family comes together with marriage and birth certificates for kids]
    REG --> INS[Get health insurance certificate, send it to HR]
    REG --> MAIL[Put your surname on a mailbox, a frontdoor</br>doorbell, and an appartment doorbell]
    MAIL --> TAX[Finanzamt will generate Steuer-ID, a.k.a. tax ID for you in 3 days, and send it via papermail in 2 weeks. You can get it faster by coming to your local Finanzamt in person]
    TAX --> STKL[In case you're married, come together to Finanzamt and explicitly tell them, which tax classes you've chosen.<br/>They will issue you two documents with your tax classes and tax ids]
    REG --> BANK[Open bank account]
    BANK --> D[Deutsche]
    BANK --> E[Sparkasse]
    BANK --> F[Commerz]
    BANK --> V[Other options/Neobanks]
    D & E & F & V --> IBAN[Get IBAN `International Bank Account Number`]
    IBAN & MAIL --> CARD[Receive bank card and its pincode with separate papermails]
    TAX & STKL --> HR1[Send scan of Tax ID and Tax Class to HR]
    REG & IBAN --> SCH[Get Schufa, credit history document. Makes sense to get it for free via paid ImmobilienScout24.de subscription <br/>Almost always it's required to be allowed for a viewing, <br/>and it's part of document list when applying for a contract]
    ACC -.-> MSFE[Ask landlord for `Mietschuldenfreiheitserklärung des Vorvermieters`]
    SCH -.-> PERM[Sign a contract for permanent accomodatior, the best case: unlimited]
    IBAN --> PERM
    MSFE -.-> |Usually, new landlord wants to know, whether you don't have any debts to previous landlord|PERM
    PERM & CAL --> I[Inform PrimeMovers to deliver your stuff]
    PERM --> REG2[Register your permanent address at town hall]
    PERM --> MAIL2[Put your surname on a mailbox, a frontdoor</br>doorbell, and an appartment doorbell]
    REG2 --> INF[Inform HR, health insurance company, bank, mobile operator, etc about your new address<br/>Very recommended: set up papermail redirects at Deutche post and PIN Mail]
    MAIL2 ----> |Birgit recommends not earlier than<br/> 2-3 month after arrival.| AMEL[Apply for permanent work permit in Ausländerbehörde]
    AGB[Ask Birgit to issue Arbeitgeberbescheinigung] -->  PERM & AMEL
    AMEL --> PMZH[Get work and residence permit for several years. It can be a bluecard, or work visa]
    PMZH --> HR2[Send scan to HR]

```

Some more information on each step:
- [Anmeldung](anmeldung.md)
- [Tax ID](finanzamt.md)
- [Schufa](schufa.md)
