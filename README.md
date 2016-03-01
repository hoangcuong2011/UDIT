# UDIT: Unsupervised Domain Induction Toolkit for Statistical Machine Translation
Given a bilingual dataset, the toolkit induces latent subdomain distributions for every source and target sentences.

To run the program: 

Step 1: Train bilingual language models with respect to latent domains

java -cp ./UDIT.jar:./trove-3.0.3.jar BilingualLMs.ProgramController [number_of_domains] [number_of_threads]

Step 2: Train the full model

java -cp ./UDIT.jar:./trove-3.0.3.jar cat.programs.SaveModel [number_of_domains] [number_of_threads]


More detail about the domain induction algorithm can be found in:

Adapting to All Domains at Once: Rewarding Domain Invariance in SMT

Hoang Cuong, Khalil Sima'an and Ivan Titov

Transactions of the Association for Computational Linguistics (TACL) 2016

You are more than welcome to hack the code!

--------------------------------------------------------------
Note that our implementation partially relies on the alignment toolkit from http://www.seas.upenn.edu/~strctlrn/CAT/CAT.html
It also heavily relies on the Kyoto Language Modeling Toolkit from http://www.phontron.com/kylm/

The first author of the TACL paper (Hoang Cuong) would like to thank the authors of the awesome toolkits, which make his life much easier!






