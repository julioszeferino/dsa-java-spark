
## Testando o ambiente spark
/home/julio/apps/spark/bin/spark-submit --master local[*] --class org.apache.spark.examples.SparkPi /home/julio/apps/spark/examples/jars/spark-examples_2.12-3.2.3.jar 80


## Compilacao
- Compilar uma aplicacao Java, permite que o arquivo .java seja convertido para bytecode e executado no SO.
- As classes seram empacotadas em um arquivo .jar
- O Maven fara a compilacao e gerenciamento das dependencias
- https://maven.apache.org/pom.html#POM_Reference 
- Escolher o compilador 11, significa usar o Java 11
- Os arquivos da compilacao sao colocados na pasta target
- Execucao da aplicacao
```bash
cd target
# validando o conteudo do arquivo
jar tf mp8-1.0.jar
# voltar para a raiz do projeto
cd ..
# executando
/home/julio/apps/spark/bin/spark-submit --class mp8.MP8App --master local[*] target/mp8-1.0.jar
```





