
# Baigiamojo darbo tyrimas ir rezultatai

Autorius: Paulius Milmantas, 2023

  

## Naudojamų failų tipai:

  

- **.ows** - Galima atsidaryti, naudojant duomenų analizės programą [Orange](https://orangedatamining.com/)

- **.ipynb** - Galima skaityti, naudojant [Google Colab](https://colab.research.google.com/) aplinkoje.

  

## Pateikti duomenų analizės failai:

 - **Transformacijos/Hidrofobiškumas.ows** - Atlikta duomenų koreliacijos ir paprastų mašininio mokymosi modelių analizė.
 - **Analize/ImportantSeqModel.ows** - Sekų kritiškumo analizė. Naudojami duomenys - *'Duomenys/Kritiskumas/test_fb11d.csv'*

## Surinkti duomenys

 - **Duomenys/Hidrofobiskumas/stats.xlsx** (nevalidūs) - Surinkti kiekvienos iteracijos duomenys:
   - Sekos pozicija MSA struktūroje. Tyrimo tikslas - sukurti metodą, gebantį prognozuoti optimalias sekų pozicijas, gaunant MSA struktūrą, su kuria AlphaFold duos tiksliausius rezultatus.
  
   - Baltymų sekos
  
   - Kiekvienos amino rūgšties skaičius sekoje
  
   - Sekų hidrofobiškumo reikšmės
  
   - **Duomenys/Hidrofobiskumas/stats.csv** - Transformuotas stats.xlxs failas, paruoštas analizei.
  
   - **Duomenys/Kritiskumas/test_fb11d.csv** - Sekų kritiškumo duomenys, gauti bandymo būdu pašalinant atitinkamas sekas.

  

## Pateiktos realizuotos transformacijų funkcijos:

  

- **Transformacijos/Hidrofobiškumas.ipynb** - Pagalbinė programa hidrofobiškumo reikšmių skaičiavimui. Priima MSA struktūrą, išveda hidrofobiškumo reikšmes kiekvienai sekai.

  

## Pagalbinės programos naudotos duomenų paruošimui

  

- **PagalbinesProgramos/Permutations.ipynb** - Generuojami duomenys, kurie turi būti paduoti AlphaFold programai.

- **PagalbinesProgramos/SequenceAnalysis.ipynb** - Analizuojamos baltymų sekos ir atrenkama jų dalis, testavimo duomenų rinkiniams generuoti.

- **PagalbinesProgramos/TimeWarping.ipynb** - Sekų ilgių suvienodinimas. Taip sekos yra paruošiamos neuroniniams tinklams vėlesniam tyrimo etapui.
