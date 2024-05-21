# iPhone UML Diagram and Implementation

## Diagrama UML

```plantuml
@startuml
skinparam classAttributeIconSize 0

interface ReprodutorMusical {
  + tocar(): void
  + pausar(): void
  + selecionarMusica(musica: String): void
}

interface AparelhoTelefonico {
  + ligar(numero: String): void
  + atender(): void
  + iniciarCorreioVoz(): void
}

interface NavegadorInternet {
  + exibirPagina(url: String): void
  + adicionarNovaAba(): void
  + atualizarPagina(): void
}

class iPhone implements ReprodutorMusical, AparelhoTelefonico, NavegadorInternet {
  + tocar(): void
  + pausar(): void
  + selecionarMusica(musica: String): void
  + ligar(numero: String): void
  + atender(): void
  + iniciarCorreioVoz(): void
  + exibirPagina(url: String): void
  + adicionarNovaAba(): void
  + atualizarPagina(): void
}
@enduml
