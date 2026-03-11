# Computação Gráfica com OpenGL

Repositório criado para armazenar exercícios e estudos da disciplina de **Computação Gráfica** do curso de **Sistemas de Informação**.

## Tecnologias utilizadas

- C++
- OpenGL
- GLUT

## Exercício 1 - Formas Básicas

Este programa cria uma janela gráfica utilizando OpenGL e desenha:

- Um quadrado amarelo
- Um triângulo verde
- Duas linhas brancas (horizontal e vertical)

### Conceitos utilizados

- Pipeline gráfico básico
- Renderização de primitivas
- Sistema de coordenadas do OpenGL
- Funções `glBegin()` e `glEnd()`

### Primitivas usadas

- `GL_QUADS`
- `GL_TRIANGLES`
- `GL_LINES`

## Como compilar

Linux:

```bash
g++ main.cpp -o programa -lGL -lGLU -lglut
