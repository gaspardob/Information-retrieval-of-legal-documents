# Evaluation-Technique-Jimini


# Mon modèle :

Mon modèle consiste à faire les étapes suivantes:
je fais l'embedding de tous les articles avec Bert
je fais l'embedding des questions + train de l'enrainement
je construis et optimise un projecteur qui rapproche la projjection de l'article et la projection de la question et qui discrimine les articles qui ne sont pas pertinents.
je recgarde ensuite les articles avec leurs projections d'embeddings les plus proches de la projection de l'embedding de la question


J'utilise Google Drive. 
il faut un dossier qui s'appelle file_path = '/content/drive/My Drive/Jimini/article_embeddings/ avec cela dedans https://drive.google.com/drive/folders/1nR1D7of6iZxezAOIwrb6uLJo42GupR4M?usp=share_link

il faut aussi telecharger questions_test, csv, questions_train.csv, bm25_negatives_train.json et articles.csv

# Installations : 

J'utilise Google Drive. 
il faut un dossier qui s'appelle file_path = '/content/drive/My Drive/Jimini/article_embeddings/ avec cela dedans https://drive.google.com/drive/folders/1nR1D7of6iZxezAOIwrb6uLJo42GupR4M?usp=share_link

il faut aussi telecharger questions_test, csv, questions_train.csv, bm25_negatives_train.json et articles.csv

!pip install datasets==2.15.0 --quiet
!pip install pandas==2.1.3 --quiet
!pip install python-terrier==0.10.0 --quiet


