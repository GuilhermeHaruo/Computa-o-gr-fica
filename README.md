# Computação Gráfica com OpenGL

Repositório criado para armazenar exercícios e estudos da disciplina de **Computação Gráfica** do curso de **Sistemas de Informação**.

## Tecnologias Utilizadas

- C++
- OpenGL
- GLUT

---

# Exercícios

## Exercício 1 — Formas Básicas

Este programa cria uma janela gráfica utilizando OpenGL e desenha:

- Um quadrado amarelo  
- Um triângulo verde  
- Duas linhas brancas (horizontal e vertical)

### Conceitos utilizados

- Pipeline gráfico básico
- Renderização de primitivas
- Sistema de coordenadas do OpenGL
- Uso das funções `glBegin()` e `glEnd()`

### Primitivas utilizadas

- `GL_QUADS`
- `GL_TRIANGLES`
- `GL_LINES`

---

## Exercício 2 — Mover um quadrado com o Teclado

**Objetivo:**  
Usar um quadrado e permitir sua movimentação utilizando as teclas **W, A, S, D** sem limitação.

**Dica:**  
Utilizar `GL_TRIANGLE_FAN` e um `for` para gerar os vértices do quadrado.

---

## Exercício 3 — Limitar Movimento dentro da Tela

**Objetivo:**  
Modificar o código para impedir que o objeto saia da área visível da janela.

**Desafio:**  
A área de visualização vai de **-1.0 a 1.0** nos eixos **X** e **Y**.  
Utilizar estruturas `if` para verificar os limites antes de atualizar as posições.

---

## Exercício 4 — Mudar Cor com Teclas Numéricas

**Objetivo:**  
Permitir que o usuário altere a cor do objeto usando as teclas numéricas.

**Teclas:**

- `1` → Vermelho
- `2` → Verde
- `3` → Azul

**Dica:**

Criar variáveis de cor:

```cpp
float r, g, b;

# Exercício 6 — Múltiplos Objetos Independentes (OpenGL)

Este exercício faz parte dos estudos da disciplina de **Computação Gráfica** do curso de **Sistemas de Informação**.

O programa cria uma janela gráfica utilizando **OpenGL** e renderiza **dois quadrados com cores diferentes**, que podem ser movimentados independentemente pelo teclado.

---

## Tecnologias Utilizadas

- C++
- OpenGL
- GLUT / FreeGLUT

---

## Objetivo do Exercício

Implementar múltiplos objetos na tela e permitir que cada um seja controlado por diferentes teclas do teclado.

Este exercício reforça conceitos como:

- Manipulação de eventos do teclado
- Controle independente de objetos
- Organização e reutilização de código
- Renderização de primitivas no OpenGL

---

## Funcionamento do Programa

O programa desenha **dois quadrados na tela**, cada um com uma cor diferente.

Cada quadrado possui seu próprio conjunto de controles para movimentação.

### Controles

| Objeto | Teclas de Movimento |
|------|------|
| Quadrado 1 | W A S D |
| Quadrado 2 | I J K L |

---

## Conceitos Utilizados

- Renderização de primitivas (`GL_QUADS`)
- Manipulação de teclado com `glutKeyboardFunc()`
- Atualização de posição de objetos
- Organização do código em funções reutilizáveis

---

## Função Reutilizável

Para evitar repetição de código, foi criada uma função para desenhar os quadrados:

```cpp
drawSquare(float x, float y, float r, float g, float b);
