# OC-Spark
Découverte de Spark grâce au cours d'OpenClassroom

## Lancement d'un script pyspark
Pour lancer un script pyspark, il faut envoyer le script python au spark-submit. Pour cela, j'ai créé un alias $SPARK_HOME qui pointe vers le dossier d'installation de spark 3.4.1 qui pour moi est : */home/guillaume/spark-3.4.1*. Une fois cela fait l'appel se fait comme suit :

    $SPARK_HOME/bin/spark-submit wordcount.py text.txt

Avec : 
- *$SPARK_HOME/bin/spark-submit* qui est l'exécutable spark
- *wordcount.py* qui est le script pyspark qui prend en paramètre un fichier texte
- *text.txt* le fichier texte utilisé par le script

Le résultat est ensuite print dans le terminal

Une autre méthode pour utiliser pyspark est d'utiliser directement le terminal grâce à la commande :
    
    PYSPARK_DRIVER_PYTHON=ipython $SPARK_HOME/bin/pyspark


## Monitorer les traitement sparks

Une manière de voir un état des lieus des lancements des traitements sparks qui ont été effectué est de lancé sparkUI. C'est une interface disponnible via navigateur à l'adresse **http://localhost:4040** *(lorsque le lancement est en local)*


## Mise en pratique de l'utilisation de Spark

Pour la mise en pratique, je me suis basé sur deux csv contenant les statistiques des joueurs de NBA sur la saison 2022-2023. Je l'ai récupéré sur Kaggle [ici](https://www.kaggle.com/datasets/vivovinco/20222023-nba-player-stats-regular?resource=download)