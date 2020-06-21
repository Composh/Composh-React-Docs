---
id: anatomy
title: Anatomy
---


Uma maneira comum de usar a estrutura da tela do Composh é ter todos os componentes dentro do <code>&lt;Container&gt;</code>

<br />


## Usage

*Sintaxe geral*

```js
import React, { Component } from 'react';
import { Container, Header, Title, Content, Footer, FooterTab, Button, Left, Right, Body, Icon, Text } from 'native-base';
export default class AnatomyExample extends Component {
  render() {
    return (
      <Container>
        <Header>
          <Left>
            <Button transparent>
              <Icon name='menu' />
            </Button>
          </Left>
          <Body>
            <Title>Header</Title>
          </Body>
          <Right />
        </Header>
        <Content>
          <Text>
            This is Content Section
          </Text>
        </Content>
        <Footer>
          <FooterTab>
            <Button full>
              <Text>Footer</Text>
            </Button>
          </FooterTab>
        </Footer>
      </Container>
    );
  }
}
```

* Todos os componentes devem ser incluídos no <code>&lt;Container&gt;</code>.

* O <code>&lt;Container&gt;</code> é composto principalmente três componentes: <code>&lt;Header&gt;</code>, <code>&lt;Content&gt;</code> and <code>&lt;Footer&gt;</code>.

* O container vem com sua folha de estilo predefinida, com uma vantagem adicional de aceitar estilos definidos pelo usuário.

<br />


## Configuration

|        Type         |    Default     | |    Options     | |    Descrição     |
| :-----------------: | :------------: | | :------------: | | :------------: |
| Header              |        -       | |        -       | | Renderiza como cabeçalho (barra de navegação) da sua tela. Valores de entrada: Botão, Título (Texto) |
| Content             |        -       | |        -       | | Representa o conteúdo principal da sua tela. Pode haver apenas um <Content>componente em uma tela. |
| Footer              |        -       | |        -       | | Renderiza como rodapé da sua tela. |