# Compilador da Linguagem TILT

### Linguagem de Programação Satírica com Análise Léxica, Sintática e Semântica

<p align="center">
  <img src="https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Java-Compiler-orange?style=for-the-badge&logo=openjdk"/>
  <img src="https://img.shields.io/badge/Compilers-Academic%20Project-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Language-TILT-red?style=for-the-badge"/>
</p>

---

## Sobre o Projeto

O **TILT** é uma linguagem de programação satírica criada com o objetivo de explorar os conceitos fundamentais da construção de compiladores. Sua sintaxe foi inspirada na ideia de um programador frustrado escrevendo código com pressa, resultando em comandos propositalmente "errados" e totalmente em letras maiúsculas.

Além da definição da linguagem, o projeto implementa um compilador capaz de realizar:

* Análise Léxica
* Análise Sintática
* Análise Semântica
* Verificação de Tipos
* Identificação de Erros e Warnings

O projeto foi desenvolvido como estudo prático dos conceitos abordados na disciplina de Compiladores.

---

## Tecnologias Utilizadas

<p align="center">
  <img src="https://skillicons.dev/icons?i=java" />
</p>

* Java
* Estruturas de Dados
* Expressões Regulares
* Análise Léxica
* Parsing
* Verificação Semântica

---

## Características da Linguagem

### Regras Gerais

* Todos os comandos devem ser escritos em MAIÚSCULO.
* Não utiliza ponto e vírgula.
* O final da linha representa o final da instrução.
* Estruturas condicionais e de repetição utilizam blocos delimitados por `{}`.

---

## Tipos Suportados

| Tipo | Descrição |
| ---- | --------- |
| ITN  | Inteiro   |
| CHRA | Caractere |
| BOL  | Booleano  |

### Exemplo

```text
ITN IDADE
CHRA LETRA
BOL ATIVO
```

---

## Entrada e Saída

### Impressão

```text
PRONT("Olá Mundo")
PRONT(IDADE)
```

### Leitura

```text
SCUM(IDADE)
```

---

## Estruturas Condicionais

### IFI

```text
IFI (IDADE >= 18) {
    PRONT("Maior de idade")
}
```

### IFI + EUSE

```text
IFI (IDADE >= 18) {
    PRONT("Maior de idade")
}
EUSE {
    PRONT("Menor de idade")
}
```

---

## Estruturas de Repetição

### WIHLE

```text
WIHLE (IDADE < 10) {
    PRONT(IDADE)
}
```

---

## Vetores

Declaração:

```text
ITN NUMEROS[10]
```

---

## Comentários

### Linha Única

```text
\\ISSO É UM COMENTÁRIO
```

### Bloco

```text
*\

BLOCO DE COMENTÁRIO

\*
```

---

## Operadores Suportados

### Aritméticos

```text
+
-
*
/
```

### Comparação

```text
==
>
<
>=
<=
```

### Lógicos

```text
AMD
ORR
```

### Booleanos

```text
TRU
FAUSE
```

---

## Verificações Semânticas

O compilador realiza diversas validações para garantir a consistência do programa.

### Variáveis não declaradas

Gera erro quando uma variável é utilizada antes de ser declarada.

### Variáveis não utilizadas

Gera warning para variáveis declaradas que nunca são utilizadas.

### Verificação de Tipos

O compilador impede operações incompatíveis como:

* ITN + CHRA
* Operações lógicas com tipos não booleanos
* Atribuições entre tipos incompatíveis

### Entrada e Saída Inválidas

Comandos `SCUM` e `PRONT` geram erro quando utilizam variáveis inexistentes.

---

## Exemplo Completo

```text
ITN CONTADOR

CONTADOR = 0

WIHLE (CONTADOR < 5) {

    PRONT(CONTADOR)

    CONTADOR = CONTADOR + 1
}
```

---

## Conceitos Aplicados

Durante o desenvolvimento deste projeto foram explorados conceitos importantes da área de compiladores:

* Análise Léxica
* Análise Sintática
* Árvores de Sintaxe
* Tabelas de Símbolos
* Verificação Semântica
* Sistemas de Tipos
* Tratamento de Erros
* Construção de Linguagens de Programação

---

## Aprendizados

Este projeto permitiu aprofundar conhecimentos em:

* Estruturas de Linguagens Formais
* Compiladores
* Autômatos
* Expressões Regulares
* Parsing
* Engenharia de Software
* Desenvolvimento em Java

---

## Melhorias Futuras

* Geração de código intermediário
* Interpretador da linguagem
* Interface gráfica para execução
* Depurador integrado
* Mais tipos de dados
* Funções e procedimentos
* Suporte a arquivos

---

## Licença

Projeto desenvolvido para fins acadêmicos e educacionais como estudo da construção de compiladores e linguagens de programação.

---
