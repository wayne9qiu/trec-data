all:trec12 trec45 nyt
	

trec12:
	mkdir trec12
	curl -s https://trec.nist.gov/data/topics_eng/topics.51-100.gz | gunzip > trec12/topics.51-100
	curl -s https://trec.nist.gov/data/topics_eng/topics.101-150.gz | gunzip > trec12/topics.101-150
	curl -s https://trec.nist.gov/data/topics_eng/topics.151-200.gz | gunzip > trec12/topics.151-200

trec45:
	mkdir trec45
	curl -s https://trec.nist.gov/data/robust/04.testset.gz | gunzip > trec45/04.testset

nyt:
	mkdir nyt
	curl -s https://trec.nist.gov/data/core/core_nist.txt > nyt/core_nist.txt

clean:
	rm -Rf trec12 trec45 nyt