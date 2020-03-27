# Conceitos do React

## Propriedades
---
<Header title="Semana OmniStack"/>

export default function Header(props){
    return (
        <header>
            <h1>{props.title}</h1>
        </header>
    );
}
---
<Header> Semana OmniStack </Header>

export default function Header({children}){
    return (
        <header>
            <h1>{children}</h1>
        </header>
    );
}

## Estado e Imutabilidade

- Informação mantida pelo componente

import React,  { useState } from 'react';

import Header from './Header';

function App() {
  const [counter, setCounter] = useState(0);

  function increment() {
    setCounter(counter + 1);
  }

  return (
    <div>
      <Header>Contador: {counter} </Header>
      <button onClick={increment}>Incrementar</button>
    </div>
  );
}

export default App;

## Pacotes instalados
 - npm install react-icons
 - npm install react-router-dom
 - npm install axios