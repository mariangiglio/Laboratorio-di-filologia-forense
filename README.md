# Filologia Forense
## _Laboratorio Università di Chieti_

## Link Utili ##
- Blocco note online. Permette di salvare documenti di solo e puro contenuto testuale. [Notepad](https://it.anotepad.com/)
- Convertitore testo> esadecimale. [Text-to-Hex](https://www.browserling.com/tools/text-to-hex)
- Editor esadecimale online. Es. [HexEd](https://hexed.it/)
- [Lista versioni word](https://it.wikipedia.org/wiki/Microsoft_Word)

### Esercizio n. 1 ###
Per capire come l'informazione ha un peso: aprire un documento di solo testo (vedi [Notepad](https://it.anotepad.com/) ) e scrivere il proprio nome. Salvare il documento e controllare quanto pesa. Il peso è uguale al numero di parole contenute. 
Da qui si capisce bene che:
1 byte = 1 carattere. 

### Esercizio n. 2 ###
Create un file rtf a partire da 0.
Tramite un editor esadecimale (es. [HexEd](https://hexed.it/) ) scrivete:
  - I _magic bytes_ tipici dell'RTF
  - Il testo che volete compaia a schermo, tradotto in formato esadecimale (vedi [Text-to-Hex](https://www.browserling.com/tools/text-to-hex) ).
  - La _chiusura_ del file RTF.
  - Salvate aggiungendo come estensione .rtf
  - Apritelo normalmente al pc.

Potete anche provare a cancellare l'estensione e vedere se qualcosa cambia nell'esadecimale oppure confrontare il vostro file con altri documenti RTF.

### Esercizio n. 3 ###
Una vera e propria prova di informatica forense. 
Da questi file illegibili trovare tramite analisi dell’esadecimale quante più informazioni possibili

## Istruzioni
- Aprire un editor esadecimale online. Es. [HexEd](https://hexed.it/)
- Scaricare uno o più file dal repository
- Il file può essere trascinato direttamente nell'editor esadecimale
- Provare a cercare informazioni utili 

## Consigli di metodo
- Ricercare i magic bytes 
- Identificare il tipo di file
- Rinominarlo aggiungendo l'estensione corretta
- Provare a datarlo facendo ricerche su internet
- Controllare ulteriori informazioni nascoste dopo la stringa di chiusura (metadati, parole chiave, informazioni personali residue, font, testo cancellato ecc.)


## Lista header
_✨Magic bytes_
- **FE 37 00 23** = Word 5.0 per Macintosh → estensione= .mcw
- **FE 37 00 1C** = Word 4.0 → estensione= .mcw
- **FE 34 00 1C** = Word 3 → estensione= .mcw
- **D0 CF 11 E0** = Word 97-2003 → estensione= .doc
- **31 BE 00 00 00 AB** = MS Word 4.0/PC file → estensione =.doc
- **FF D8 FF** = File immagine → estensione =.jpeg
- **7B 5C 72 74 66 31 5C 61 6E 73 69 0A** = File RTF → estensione =.rtf 

## Stringa di fine testo (EOT)
**75 00** → stringa di fine testo. Il materiale dopo è stato probabilmente aggiunto dopo la chiusura



