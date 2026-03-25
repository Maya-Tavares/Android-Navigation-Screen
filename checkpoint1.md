# Checkpoint 1 — Navigation Compose

## Descrição do projeto

Este projeto consiste em uma aplicação Android desenvolvida com **Jetpack Compose**, com foco na navegação entre telas utilizando o **Navigation Compose**.

O aplicativo possui quatro telas principais:

- Login
- Menu
- Pedidos
- Perfil

A navegação entre essas telas é controlada por um `NavController`, permitindo a passagem de parâmetros entre rotas.

---

## Objetivo da prova

De acordo com o enunciado da atividade :contentReference[oaicite:0]{index=0}, o objetivo é:

- Evoluir um projeto já existente
- Aplicar conceitos de navegação entre telas com Jetpack Compose
- Trabalhar com passagem de parâmetros (obrigatórios e opcionais)
- Demonstrar domínio técnico e entendimento do código

## Principais arquivos

O projeto está dividido em:

MainActivity: ponto de entrada do app e local onde a navegação é configurada;
Screens: arquivos que representam as telas;
Gradle: onde está a dependência necessária para usar o Navigation Compose.

Arquivos principais:

Main.kt
LoginScreen.kt
MenuScreen.kt
PedidosScreen.kt
PerfilScreen.kt
---

## Configuração da navegação

A navegação é configurada na `MainActivity` utilizando os seguintes componentes:

### NavController

implementation("androidx.navigation:navigation-compose:2.6.0")

Essa biblioteca permite usar:

rememberNavController()
NavHost
composable
navArgument
NavType

Sem essa dependência, não seria possível configurar a navegação entre telas com Compose.

```kotlin
val navController = rememberNavController()