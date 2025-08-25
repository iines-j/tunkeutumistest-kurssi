# h1 Kybertappoketju
> Kill Chain #1: Recon. Porttiskannauksen lisäksi alamme rakentaa hakkerilabraa.

- x)[ Lue ja tiivistä ](#x-lue-ja-tiivistä)
- a)[ Asenna Kali ](#a-asenna-kali)
- b)[ Irrota verkosta ](#b-irrota-verkosta)
- c)[ Porttiskannaus ](#c-porttiskannaus)
- d)[ Demonit ](#d-demonit)
- e)[ Metasploitable 2 ](#e-metasploitable-2)
- f)[ Virtuaaliverkko ](#f-virtuaaliverkko)
- g)[ Etsi Metasploitable ](#g-etsi-metasploitable)
- h)[ Portit hyökkääjälle ](#h-portit-hyökkääjälle)
- [Lähteet](#lähteet)


Tehtäviä saa aloittaa vasta, kun on hyväksynyt kurssin säännöt. Koneet on eristettävä Internetistä hyökkäysten harjoittelun ajaksi.

Tehtävät ovat virallisia vasta, kun ne on annettu tehtäväksi. Niitä ei tule aloittaa etukäteen, koska niiden sisältö voi vielä muuttua olennaisesti.

## x) Lue ja tiivistä
> (Tässä x-alakohdassa ei tarvitse tehdä testejä tietokoneella, vain lukeminen tai kuunteleminen ja tiivistelmä riittää. Tiivistämiseen riittää muutama ranskalainen viiva.)
        Herrasmieshakkerit (RSS) tai Darknet Diaries (RSS) , yksi vapaavalintainen jakso jommasta kummasta. Voi kuunnella myös lenkillä, pyykiä viikatessa tms. Siisti koti / hyvä kunto kaupan päälle.
        Hutchins et al 2011: Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains, chapters Abstract, 3.2 Intrusion Kill Chain.
        € Santos et al: The Art of Hacking (Video Collection): 4.3 Surveying Essential Tools for Active Reconnaissance. Sisältää porttiskannauksen. 5 videota, yhteensä noin 20 min.
        KKO 2003:36.

## a) Asenna Kali
> (Jos asennuksessa ei ole mitään ongelmia tai olet asentanut jo aiemmin, tarkkaa raporttia tästä alakohdasta ei tarvita. Kerro silloin kuitenkin, mikä versio ja millä asennustavalla. Jos on ongelmia, niin tarkka ja toistettava raportti).

## b) Irrota verkosta 
> Todista testein, että virtuaalikone ei saa yhteyttä Internetiin (esim. 'ping 8.8.8.8')

## c) Porttiskannaus
> Porttiskannaa 1000 tavallisinta tcp-porttia omasta koneestasi (nmap -T4 -A localhost). Selitä komennon paramterit. Analysoi ja selitä tulokset.

## d) Demonit
>  Asenna kaksi vapaavalintaista demonia ja skannaa uudelleen. Analysoi ja selitä erot.

## e) Asenna Metasploitable 2 

## f) Virtuaaliverkko
> Tee koneiden välille virtuaaliverkko. Jos säätelet VirtualBoxista
        Kali saa yhteyden Internettiin, mutta sen voi laittaa pois päältä
        Kalin ja Metasploitablen välillä on host-only network, niin että porttiskannatessa ym. koneet on eristetty intenetistä, mutta ne saavat yhteyden toisiinsa
        Vaihtoehtoisesti voit tehdä molempien koneiden asennuksen ja virtuaaliverkon vagrantilla. Silloin molemmat koneet samaan Vagrantfile:n.

## g) Etsi Metasploitable 
> porttiskannaamalla (nmap -sn). Tarkista selaimella, että löysit oikean IP:n - Metasploitablen weppipalvelimen etusivulla lukee Metasploitable.

## h) Portit hyökkääjälle
> Porttiskannaa Metasploitable huolellisesti ja kaikki portit (nmap -A -T4 -p-). Poimi 2-3 hyökkääjälle kiinnostavinta porttia. Analysoi ja selitä tulokset näiden porttien osalta.
