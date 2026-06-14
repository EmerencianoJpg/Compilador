# Compilador da Linguagem TILT

### Linguagem de Programação Satírica Inspirada em C

<p align="center">
  <img src="https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Compiler-Project-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Language-TILT-red?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Syntax-C--Inspired-orange?style=for-the-badge"/>
</p>

---

## Sobre o Projeto

O **TILT** é uma linguagem de programação satírica inspirada na sintaxe da linguagem C e criada com o objetivo de explorar os conceitos fundamentais da construção de compiladores.

Sua proposta é simular um código escrito por um programador frustrado e com pressa, utilizando palavras-chave propositalmente incorretas e comandos totalmente em letras maiúsculas.

Além da definição da linguagem, o projeto implementa um compilador capaz de realizar:

* Análise Léxica
* Análise Sintática
* Análise Semântica
* Verificação de Tipos
* Identificação de Erros e Warnings

O projeto foi desenvolvido como estudo prático dos conceitos de Linguagens Formais e Compiladores.

---

## Tecnologias Utilizadas

* Compiladores
* Linguagens Formais
* Análise Léxica
* Análise Sintática
* Análise Semântica
* Tabela de Símbolos
* Expressões Regulares
* Estruturas de Dados

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

    IDADE = IDADE + 1
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
*\\
BLOCO DE COMENTÁRIO
\\*
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

O compilador realiza diversas validações para garantir a consistência dos programas escritos na linguagem.

### Variáveis Não Declaradas

Gera erro quando uma variável é utilizada antes de sua declaração.

### Variáveis Não Utilizadas

Gera warning para variáveis declaradas que nunca são utilizadas.

### Verificação de Tipos

O compilador impede operações incompatíveis como:

* ITN + CHRA
* Operações lógicas utilizando tipos não booleanos
* Atribuições entre tipos incompatíveis

### Entrada e Saída Inválidas

Comandos `SCUM` e `PRONT` geram erro quando utilizam variáveis inexistentes.

---

## Exemplos de Código

```text
ITN CONTADOR

CONTADOR = 0

WIHLE (CONTADOR < 5) {

    PRONT(CONTADOR)

    CONTADOR = CONTADOR + 1
}
```

---

```text
ITN IDADE

SCUM(IDADE)

IFI (IDADE >= 18) {

    PRONT("MAIOR DE IDADE")

}
EUSE {

    PRONT("MENOR DE IDADE")

}
```

---

## Objetivo Acadêmico

O projeto foi desenvolvido com o objetivo de aplicar na prática os conceitos estudados em Linguagens Formais e Compiladores, abrangendo desde a definição da gramática da linguagem até a validação semântica dos programas escritos em TILT.

---

## Licença

Projeto desenvolvido para fins acadêmicos e educacionais como estudo da construção de compiladores e linguagens de programação.

---
