---
id: accordion
title: Accordion
---


## Accordion

Alterne a visibilidade do conteúdo entre os itens da tela. O Accordion alterna entre vários blocos de texto com um único clique.

O Accordion é renderizado com ícones predefinidos na alternância entre o bloco de texto, o cabeçalho e o estilo do conteúdo.

<br />


**Contents:**
* [Icon and Expanded Icon](Components.md#accordion-icon-headref)
* [Icon and Expanded Icon style](Components.md#accordion-icon-style-headref)
* [Header and Content style](Components.md#accordion-header-content-headref)
* [Custom Header and Content](Components.md#accordion-custom-header-content-headref)

*Sintaxe geral*

```js
import React, { Component } from "react";
import { Container, Header, Content, Accordion } from "native-base";
const dataArray = [
  { title: "First Element", content: "Lorem ipsum dolor sit amet" },
  { title: "Second Element", content: "Lorem ipsum dolor sit amet" },
  { title: "Third Element", content: "Lorem ipsum dolor sit amet" }
];
export default class AccordionExample extends Component {
  render() {
    return (
      <Container>
        <Header />
        <Content padder>
          <Accordion dataArray={dataArray} expanded={0}/>
        </Content>
      </Container>
    );
  }
}
```


**Configuration**<br />
| Property          | Default    | Option           | Description                                                                                                          |
|-------------------|------------|------------------|----------------------------------------------------------------------------------------------------------------------|
|     dataArray     | Array      | -                | Matriz de blocos de dados para renderizar iterativamente                                                             |
| expanded          | -          | -                | Índice do conjunto de acordeão aberto                                                                                |
| headerStyle       | -          | -                | Cabeçalho de acordeão de estilo                                                                                      |
| contentStyle      | -          | -                | Estilo de conteúdo de acordeão                                                                                       |
| icon              | arrow-down | usuário definido | Ícone quando o acordeão é fechado                                                                                    |
| expandedIcon      | arrow-up   | usuário definido | Ícone quando o acordeão está aberto                                                                                  |
| iconStyle         | -          | usuário definido | Estilo do ícone quando o acordeão é fechado                                                                          |
| expandedIconStyle | -          | usuário definido | Estilo do ícone quando o acordeão está aberto                                                                        |
| renderHeader      | -          | -                | Design personalizado do cabeçalho Acordeão                                                                           |
| renderContent     | -          | -                | Design personalizado do conteúdo do acordeão                                                                         |
| onAccordionOpen   | Função     | -                | Retorno de chamada que é executado quando o Acordeão é aberto. Ele fornece dois metadados adicionais: item e índice  |
| onAccordionClose  | Função     | -                | Retorno de chamada que é executado quando o acordeão é fechado. Ele fornece dois metadados adicionais: item e índice |