# db-g1

-------ES 1 -----------

SELECT nome from clienti
WHERE nome = 'Mario'

-------ES 2 ---------

SELECT nome, cognome from clienti
WHERE anno_nascita = 1982

-------ES 3 ---------

SELECT count(*) from fatture
WHERE iva = '20'

-------ES 4 ---------

SELECT * 
FROM prodotti 
WHERE EXTRACT(YEAR FROM data_attivazione) = 2017
AND (in_produzione = TRUE OR in_commercio = TRUE);
