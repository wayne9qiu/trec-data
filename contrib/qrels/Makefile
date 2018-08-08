all: trec12 trec45 nyt
	
trec12: 
	mkdir trec12
	cd trec12; curl -O https://trec.nist.gov/data/qrels_eng/qrels.51-100.disk1.disk2.parts1-5.tar.gz; tar xzf qrels.51-100.disk1.disk2.parts1-5.tar.gz; gunzip *.gz; rm -f *.tar
	cd trec12; curl -O https://trec.nist.gov/data/qrels_eng/qrels.101-150.disk1.disk2.parts1-5.tar.gz; tar xzf qrels.101-150.disk1.disk2.parts1-5.tar.gz; gunzip *.gz; rm -f *.tar
	cd trec12; curl -O https://trec.nist.gov/data/qrels_eng/qrels.151-200.201-250.disks1-3.all.tar.gz; tar xzf qrels.151-200.201-250.disks1-3.all.tar.gz; gunzip *.gz; rm -f *.tar *interactive*

trec45: 
	mkdir trec45
	cd trec45; curl -O https://trec.nist.gov/data/robust/qrels.robust2004.txt

nyt:
	mkdir nyt
	cd nyt; curl -O https://trec.nist.gov/data/core/qrels.txt

clean:
	rm -Rf trec12 trec45 nyt