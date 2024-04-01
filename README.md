# Evaluation-Technique-Jimini


# Mon modèle :

Mon modèle consiste à faire les étapes suivantes:
je fais l'embedding de tous les articles avec Bert
je fais l'embedding des questions + train de l'enrainement
je construis et optimise un projecteur qui rapproche la projjection de l'article et la projection de la question et qui discrimine les articles qui ne sont pas pertinents.
je recgarde ensuite les articles avec leurs projections d'embeddings les plus proches de la projection de l'embedding de la question



# Installations : 

J'utilise Google Drive. 
il faut un dossier qui s'appelle file_path = '/content/drive/My Drive/Jimini/article_embeddings/ avec les différents fichiers du github à l'interieur.

Ainsi, on peut importer les embeddings des 22k articles (et notamment leurs projections), ainsi que le projecteur P_q, 

il faut aussi telecharger questions_test, csv, questions_train.csv, bm25_negatives_train.json et articles.csv de la base de donnée https://huggingface.co/datasets/maastrichtlawtech/bsard/tree/main

Il suffit ensuite de charger P_q_ex.pth et all_projected_article_embeddings_ex.pt. 


!pip install datasets==2.15.0 --quiet
!pip install pandas==2.1.3 --quiet
!pip install python-terrier==0.10.0 --quiet


