# Criando um Aplicativo de Portfólio com React Native

## Introdução
Um aplicativo de portfólio é essencial para qualquer desenvolvedor mostrar seu trabalho e habilidades a potenciais empregadores ou clientes. Neste artigo, vou guiá-lo passo a passo na criação de um aplicativo de portfólio usando React Native. Vamos organizar nosso projeto em módulos para facilitar a manutenção e expansão.

## Pré-requisitos
Antes de começarmos, certifique-se de ter instalado o seguinte:

1. **Node.js e npm**: Vamos usar o Node.js para criar nosso aplicativo.
2. **React Native CLI**: Instale o React Native Command Line Interface para criar e gerenciar projetos React Native.
3. **Expo CLI (opcional)**: O Expo é uma ferramenta que facilita o desenvolvimento React Native. Você pode instalá-lo globalmente com `npm install -g expo-cli`.

## Passo 1: Configuração do Projeto
Vamos criar um novo projeto React Native chamado "MeuPortfolioApp". Abra o terminal e execute os seguintes comandos:

```bash
npx react-native init MeuPortfolioApp
cd MeuPortfolioApp
```

## Passo 2: Estrutura do Projeto
Dentro do diretório do projeto, crie uma estrutura básica para organizar os módulos:

- `src/`: Pasta principal do código-fonte.
  - `components/`: Aqui ficarão os componentes reutilizáveis.
  - `screens/`: Cada tela do aplicativo terá seu próprio arquivo aqui.
  - `navigation/`: Configuração de navegação entre telas.
  - `assets/`: Imagens, ícones e outros recursos.
  - `App.js`: Ponto de entrada do aplicativo.

## Passo 3: Criando Componentes
Vamos criar alguns componentes básicos:

### Navbar
```jsx
// src/components/Navbar.js
import React from 'react';
import { View, Text } from 'react-native';

const Navbar = () => {
  return (
    <View>
      <Text>Meu Portfólio</Text>
    </View>
  );
};

export default Navbar;
```

### Sobre Mim
```jsx
// src/screens/AboutScreen.js
import React from 'react';
import { View, Text } from 'react-native';

const AboutScreen = () => {
  return (
    <View>
      <Text>Sou um desenvolvedor apaixonado por tecnologia...</Text>
    </View>
  );
};

export default AboutScreen;
```

## Passo 4: Configurando a Navegação
Vamos usar o React Navigation para navegar entre as telas. Instale-o com:

```bash
npm install @react-navigation/native @react-navigation/stack
```

Configure a navegação no arquivo `src/navigation/AppNavigator.js`.

## Passo 5: Estilizando e Adicionando Conteúdo
Estilize seus componentes usando CSS-in-JS ou uma biblioteca como Styled Components. Adicione informações sobre você, projetos, habilidades e links de contato nas telas.

## Conclusão
Parabéns! Você criou um aplicativo de portfólio básico com React Native. Personalize-o, adicione mais telas e recursos conforme sua necessidade. Agora você tem uma maneira elegante de mostrar seu trabalho aos outros!
