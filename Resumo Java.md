### Estudando Java
Write Once, Run Anywhere (WORA) - "Escreva uma vez, execute em qualquer lugar", é o lema principal do Java e o motivo pelo qual ele se tornou tão popular no mundo da tecnologia.

## Sintaxe (A Gramática)
  É um conjunto de regras que você deve seguir para que o compilador do JDK entenda seu código. Java é uma 
linguagem Case Sensitive(faz diferença entre maiúsculas e minúsculas) e todo instrução termina com ponto e virgula( ; ).
* **Classes:** Tudo em Java acontece dentro de uma classe. O nome do arquivo deve ser igual o nome da classe.
* **Méetodo Main:** É a porta de entrada. Sem ele, o programa não "começa".
* **Chaves{}:** Delimitam onde começa e termina um bloco de código(como uma classe ou um método).

### Código em Java
```java
public class OlaMundo { // Nome da Classe
    public static void main(String[] args) { // Método de entrada
        System.out.println("Olá, Java!"); // Instrução (Sintaxe)
    }
}
```
## Pacote(A Organização)
Os Packages(pacotes) funcionam como "pastas" para agrupar classes relacionadas.
* **Evita conflitos:** Você pode ter duas classes chamadas Calculadora, desde que estejam em pacotes diferentes (ex: financeiro.Calculadora e escalar.Calculadora).
* **Declaração:** Deve ser a primeira linha do seu código: package br.com.meuprojeto;

## Biblioteca (As Ferramentas Prontas)  
Biblioteca são conjuntos de pacotes e classes já prontos que você pode importar para seu projeto.
* **Java Standard Edition(SE):** É uma biblioteca padrão que vem no JDK (ex: para ler o teclado, usar datas ou até fazer cálculos matemáticos).
* **Como usar:** Você pode usar o comando import no topo do arquivo.
Ex: *import java.util.Scanner*; (importa a ferramenta para ler o que o usuário digita).

## Principal uso de JDK(Java Development Kit)
  Lembre dele como um **"Kit de ferramentas"** que todo desenvolvedor presa para criar programas 
em Java. Sem ele até da para rodar um programa pronto, mas você não consegue escrever ou transformar
seu código em algo que o computador entenda.

## Principal função da JVM(Java Virtual Machine)
  É o **coração** ou *motor* que executa o código Java em qualquer dispositivo ou sistema operacional.
Para entender melhor, o computador não entende diretamente o código que você escreve em Java. 
Ele precisa de um intermediário que transforme as instruções do programa em algo que o 
hardware(processador) consiga processar.

## Principal função de JRE(Java Runtime Environment)
  É o **ambiente de execução**, se você quer apenas rodar um programa de Java no seu computador, você precisa do JRE. Nele você não cria arquivos(não compila), ele serve para você rodar o sistema mas você não pode criar um novo código.

## Java Standard Edition (SE), Java Enterprise Edition (EE) e Java Micro-Edition (ME)
* **Java SE (Standard Edition):** É o núcleo do Java. Tudo o que conversamos até agora (JDK, JVM, JRE) faz parte do Java SE. Ele contém as bibliotecas fundamentais para qualquer desenvolvedor.
* **Java EE (Enterprise Edition) – Atualmente Jakarta EE:** É uma camada construída em cima do Java SE. Ela foi feita para grandes empresas que precisam de sistemas complexos, seguros e que aguentem milhares de acessos ao mesmo tempo.
* **Java ME (Micro Edition):** Como o nome sugere, é uma versão "enxuta" feita para dispositivos com pouca memória e processamento.









