# Modelagem e Diagramação do iPhone com UML

Este projeto tem como objetivo modelar e diagramar a representação UML do componente iPhone, abrangendo suas funcionalidades como Reprodutor Musical, Aparelho Telefônico e Navegador na Internet.

## Contexto

Com base no vídeo de lançamento do iPhone de 2007, foi elaborada a diagramação das classes e interfaces utilizando uma ferramenta UML. Em seguida, as classes e interfaces foram implementadas em Java.

- **Lançamento iPhone 2007:** [Assista ao vídeo](https://www.youtube.com/watch?v=9hUIxyE2Ns8)
  - *Minutos relevantes:* 00:15 até 00:55

## Funcionalidades Modeladas

As principais funcionalidades modeladas no projeto incluem:

- **Reprodutor Musical (Interface `ReprodutorMusical`):**
  - `tocar()`
  - `pausar()`
  - `selecionarMusica(String musica)`

- **Aparelho Telefônico (Interface `AparelhoTelefonico`):**
  - `ligar(String numero)`
  - `atender()`
  - `iniciarCorreioVoz()`

- **Navegador de Internet (Interface `NavegadorInternet`):**
  - `exibirPagina(String url)`
  - `adicionarNovaAba()`
  - `atualizarPagina()`

## Diagrama UML

A estrutura do iPhone foi representada no seguinte diagrama UML:

![UML](https://raw.githubusercontent.com/felipefortu33/UML_Iphone/refs/heads/master/Captura%20de%20tela%202025-04-05%20184640.png)

```plantuml

@startuml
interface ReprodutorMusical {
  +tocar()
  +pausar()
  +selecionarMusica(musica: String)
}

interface AparelhoTelefonico {
  +ligar(numero: String)
  +atender()
  +iniciarCorreioVoz()
}

interface NavegadorInternet {
  +exibirPagina(url: String)
  +adicionarNovaAba()
  +atualizarPagina()
}

class iPhone implements ReprodutorMusical, AparelhoTelefonico, NavegadorInternet {
  // Implementações dos métodos
}
@enduml
  


