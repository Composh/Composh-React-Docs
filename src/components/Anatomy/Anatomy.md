---
id: anatomy
title: Anatomy
---


Uma maneira comum de usar a estrutura da tela do Composh é ter todos os componentes dentro do <code>&lt;Container&gt;</code>

<br />


## Usage

*General Syntax*

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

<br />


* Todos os componentes devem ser incluídos no <code>&lt;Container&gt;</code>.

* O <code>&lt;Container&gt;</code> é composto principalmente três componentes: <code>&lt;Header&gt;</code>, <code>&lt;Content&gt;</code> and <code>&lt;Footer&gt;</code>.

* O container vem com sua folha de estilo predefinida, com uma vantagem adicional de aceitar estilos definidos pelo usuário.


## Configuration

<br />

```js
    <table class="table table-bordered">
        <thead>
            <tr>
                <th>Property</th>
                <th>Default</th>
                <th>Option</th>
                <th width="50%">Description</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Header</td>
                <td> - </td>
                <td> - </td>
                <td>Renders as Header (navbar) of your screen.<br />
                    Input values: Button, Title (Text).
                </td>
            </tr>
            <tr>
                <td>Content</td>
                <td> - </td>
                <td> - </td>
                <td>Represents the main content of your screen.<br />
                    There can be only one <code style="background-color: #FFF">&lt;Content></code> component in a screen.
                </td>
            </tr>
            <tr>
                <td>Footer</td>
                <td> - </td>
                <td> - </td>
                <td>Renders as Footer of your screen.<br />
                    Input values: FooterTab
                    </a>
                </td>
            </tr>
        </tbody>
    </table>
    <br />
```