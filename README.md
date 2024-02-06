# Resumo

Construção de um analisador léxico simples utilizando Flex.

A linguagem aceita pela grámatica é similar à Linguagem Java, como exemplo ela identifica os seguintes tokens:

```
RESERVADA "class"|"public"|"static"|"void"|"main"|"String"|"extends"|"if"|"while"|"System.out.println"|"else"|"new"|"this"|"return"|"length"
TIPO "int"|"boolean"
OPERADOR  "&&"|"<"|"+"|"-"|"*"|"="
```

# Pré-Requisitos

- Flex GNU
- Ferramentas de Compilação de Código Fonte C, como **gcc**

# Como utilizar

Em um terminal utilize os seguintes comando:

```
flex gramatica.l
gcc -o analisador lex.yy.c
analisador < teste.txt
analisador < small_teste.txt
```
