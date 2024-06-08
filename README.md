Classificació Multiclasse de Mamografies Mitjançant Aprenentatge Profund


Aquest és el repostori corresponent al Treball de Final de Màster del màster de Ciència de Dades de la UOC (2024)

A la carpeta src es troben els notebooks per executar el projecte. 
El fitxer requeriments.txt conté les llibreries per executar-los correctament.
Quan així s'indica al títol del notebook, aquest està preparat per executar en entorn de Google Colab amb GPU.
Els arxius de la carpeta src son els següents:

1 - Unificació datasets.ipynb --> Aquest notbook conté els enllaços per obtenir els datasets, homogeneitzar les imatges i el recolliment dels paths i les característiques en un arxiu .csv
2 - Anàlisi exploratori.ipynb --> Anàlisi exploratori del dataset resultant
3 - Preprocessament imatges_3CLASS.ipynb --> Aquest notebook preprocessa les imatges dels diferents datasets per a l'entrenament. El resultat son arrays de numpy per ser entrenades (en el nostre cas a Google Colab)
4 - Preprocessament imatges patches.ipynb --> Aquest notebook preprocessa les imatges retallant patches de les zones d'interes. S'obtenen arrays de numpy per ser entrenades a Google Colab
5 - Models amb mamografies completes-COLAB.ipynb --> Notebook per a l'entrenament de les imatges senceres. Pren com entrada els arrays de numpy i obté un model entrenat.
6 - Models amb patches-COLAB.ipynb --> Notebook per a l'entrenament de les imatges retallades. Pren com entrada els arrays de numpy i obté un model entrenat.
7 - Hiperparametrització full mammo-COLAB.ipynb --> Hiperparametrització dels models per a les imatges senceres
8 - Hiperparametrització patches-COLAB.ipynb --> Hiperparametrització dels models per a les imatges retallades
9 - Model_ensembling-COLAB.ipynb --> Notebook per realitzar ensembling dels millors models obtinguts en les imatges senceres. 


Addicionalment es proporcionen els enllaços a Zenodo, disponibles sota petició:

Els arrays de numpy i els arxius csv amb els index d'entrenament, validació i test per a entrenar les imatges senceres:
https://zenodo.org/records/11528223

Els arrays de numpy i els arxius csv amb els index d'entrenament, validació i test per a entrenar les imatges retallades:
https://zenodo.org/records/11528282

Els tres millors models obtinguts en l'entrenament de imatges senceres, corresponents als models preentrenats amb Inception, VGG19 i EfficientNetB2:
https://zenodo.org/records/11528115


