# Engeto project no.3 (Election scraper)
Third project - Python Academy from Engeto.

## Description of the project
This project extracts results of the 2017 parliamentary elections from the website on the [link](https://www.volby.cz/pls/ps2017nss/ps3?xjazyk=CZ).

## Required Libraries
Required libraries for running this program are in the file `requirements.txt`. 
For installation of these libraries, I suggest using a new virtual environment and with the official package manager run it as shown below:
```
$ pip3 --version                    # verify manager version 
$ pip3 install -r requirements.txt  # instalation of the libraries
```

## Running the program
Running the file `main.py` in the CLI requires two mandatory arguments.
```
python main.py <link_of_territorial_unit> <name_of_the_output_file>
```
Data will download to the file with file name extension `.csv`.

## Arguments
Election results of Jihočeský region, district České Budějovice:

1. argument:  `https://www.volby.cz/pls/ps2017nss/ps31?xjazyk=CZ&xkraj=3&xnumnuts=3101`
2. argument:  `Ceske_Bud.csv`

###### Demonstration of the program:
```
(venv) PS C:\Users\lukas\PycharmProjects\Engeto projekt č.3> python main.py "https://www.volby.cz/pls/ps2017nss/ps31?xjazyk=CZ&xkraj=3&xnumnuts=3101" , "Ceske_Bud.csv"
```

###### Process of downloading:
```
Stahuji data z: https://www.volby.cz/pls/ps2017nss/ps31?xjazyk=CZ&xkraj=3&xnumnuts=3101
Stažená data ukládám do souboru: Ceske_Bud.csv
Ukončuji program.
```

###### Partial output:
```
code;location;registered;envelopes;valid;Občanská demokratická strana;Řád národa - Vlastenecká unie;CESTA ODPOVĚDNÉ SPOLEČNOSTI;Česká str.sociálně demokrat.;Radostné Česko;STAROSTOVÉ A NEZÁVISLÍ;Komunistická str.Čech a Moravy;Strana zelených;ROZUMNÍ-stop migraci,diktát.EU;Strana svobodných občanů;Blok proti islam.-Obran.domova;Občanská demokratická aliance;Česká pirátská strana;Referendum o Evropské unii;TOP 09;ANO 2011;Dobrá volba 2016;SPR-Republ.str.Čsl. M.Sládka;Křesť.demokr.unie-Čs.str.lid.;Česká strana národně sociální;REALISTÉ;SPORTOVCI;Dělnic.str.sociální spravedl.;Svob.a př.dem.-T.Okamura (SPD);Strana Práv Občanů
215;České Budějovice;110936;71261;70883;9908;69;63;4417;70;3736;5294;1195;410;1526;55;156;7601;57;4675;19528;64;106;3525;81;1202;172;122;6616;235
216;Hluboká nad Vltavou;6274;4109;4096;722;3;1;283;11;198;362;59;30;68;2;9;429;2;216;1033;2;8;210;2;50;14;13;360;9
217;Lišov;4745;3108;3094;340;4;4;143;3;421;266;32;16;40;3;6;235;3;107;827;1;6;202;2;37;13;4;376;3
...
```
