# Ekaterina Rubanskaja. Prekybos įmonių duomenų tyrimas naudojant SQL.

Visas darbas susideda iš šešių etapų ir padarytas online-aplinkoje. Kiekvienas sekantis etapas yra prieš jo einančio etapo tęsinys.

## Užduoties aprašymas:

	Parengti analitinę ataskaitą apie prekybos įmonės veiklą. 
  
  Duomenys: https://dbfiddle.uk/sI63XXnh?hide=1

**1 etapas.** Gautų duomenų analizė.

1. Išnagrinėti duomenų lentelės struktūrą, nustatyte stulpelių sąrašą ir duomenų tipus.
2. Nustatyti eilučių skaičių.
3. Išnagrinėti kiekvieno lauko duomenis.
4. Pateikti bendrą nagrinėjamų duomenų tekstinį aprašymą.

  Pirmo etapo darbas čia: https://dbfiddle.uk/YkiRJq4M?hide=1024

**2 etapas.** Duomenų klaidų taisymas.

1. Rasti ir ištaisykite visas duomenų klaidas.
2. Ištaisę klaidas, nustatyti kai kurias duomenų charakteristikas:
  1. Lentelės eilučių skaičius,
  2. Kiekvienos produktų kategorijos paskirstymo eilučių skaičius,
  3. Kiekvieno gamintojo paskirstymo linijų skaičius,
  4. Minimali, maksimali ir vidutinė cnt stulpelio vertės,
  5. Minimali, maksimali ir vidutinė stulpelio price vertės.

  Antro etapo darbas čia: https://dbfiddle.uk/V4zGjJS0?hide=4294967296

  **3 etapas.** Finansinių rodiklių analizė.

  	Išskirkti šiuos rodiklius:
- pirkimų dinamiką pagal mėnesį,
- įmonės pelną per visą laikotarpį,
- įmonės pardavimų rodiklių dinamiką pagal mėnesį,
- mėnesinė finansinių srautų dinamiką,
ir taip pat pridėti finansinės veiklos ataskaitą pagal produktų kategorijas.

	Trečio etapo darbas čia: https://dbfiddle.uk/VHRAyrOa?hide=17592186042368. Prie šito trečio etapo pridedama grafinė dalis, padaryta Power BI Desktop'e.

**4 etapas.** Duomenų bazės struktūros modernizavimas.

1. Sukurkite šias nuorodų lenteles:
  - order_type
  - product_category
  - product
  - manufacturer
2. Užpildykite sukurtas nuorodų lenteles duomenimis iš atitinkamų invoice_order_operations lentelės stulpelių.
3. Sukurkite duomenų lentelę operations_data su tokia struktūra:

<img width="956" height="726" alt="image" src="https://github.com/user-attachments/assets/b57bd9d0-5f54-43ea-900a-5cee2d651f2f" />

4. Užpildykite lentelę operations_data duomenimis iš lentelės invoice_order_operations ir visų nuorodų lentelių.
5. Naujoje lentelėje operations_data atlikite užklausas, kurios nustato kai kurias duomenų charakteristikas. Įrašykite rezultatus į lentelę:

<img width="1440" height="551" alt="image" src="https://github.com/user-attachments/assets/97918329-e929-4918-ad8d-89494e8e4a73" />

  Ketvirto etapo darbas čia: https://dbfiddle.uk/bONvUwNU?hide=144115188075847680

**5 etapas.** Sandėlio likučių apskaičiavimas.

  Išanalizuokite prekių judėjimą per visą laikotarpį ir apskaičiuokite dabartinę kiekvienos prekės sandėlio būseną.

  Penkto etapo darbas čia: https://dbfiddle.uk/uAzcFjsK?hide=4611686018427388000

**6 etapas.** Papildomos duomenų dalies importavimas.

  Gavom papildomas duomenis https://dbfiddle.uk/uZE33Za3?hide=1 , kur operations_data tai duomenys, kurios jau apdorotos, ir invoice_order_raw , tai nauja prekybos įmonės duomenų partija.

**Tikslas:**
1. Apdoroti duomenis iš lentelės invoice_order_raw ir pridėkite juos prie lentelės operation_data.
2. Įtraukus duomenis į lentelę „operation_data“, apskaičiuoti šiuos rodiklius:
  - Lentelės eilučių skaičius,
  - Kiekvienos produktų kategorijos paskirstymo eilučių skaičius,
  - Kiekvieno gamintojo paskirstymo linijų skaičius,
  - Minimali, maksimali ir vidutinė cnt stulpelio vertės,
  - Minimali, maksimali ir vidutinė stulpelio price vertės.

  Šešto etapo darbas čia: https://dbfiddle.uk/cE0_9D4-?hide=8388608
  
