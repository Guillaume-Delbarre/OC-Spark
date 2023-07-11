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
