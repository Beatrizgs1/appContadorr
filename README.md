# 📱 App Contador

**Desenvolvido por: Beatriz Gonçalves de Souza**

Projeto desenvolvido para a atividade de Android, utilizando **Kotlin**, **Jetpack Compose** e **Material 3**.

A ideia do aplicativo é simples: mostrar um número na tela e permitir que ele aumente cada vez que o usuário clicar no botão **Adicionar**.

---

## 🎯 Objetivo do projeto

O objetivo foi criar uma tela simples de contador e entender alguns conceitos básicos do desenvolvimento Android com Jetpack Compose.

No aplicativo, o contador começa em **0**. Quando o botão é pressionado, o valor aumenta em 1.

Exemplo:

```text
Contador: 0
      ↓
  Adicionar
      ↓
Contador: 1
      ↓
  Adicionar
      ↓
Contador: 2
```

---

## 🛠️ Tecnologias utilizadas

* **Kotlin** – linguagem utilizada no desenvolvimento.
* **Jetpack Compose** – utilizado para criar a interface da tela.
* **Material 3** – utilizado nos componentes e no tema visual.
* **Android SDK** – base para o desenvolvimento do aplicativo Android.
* **Gradle** – utilizado para configurar e organizar o projeto.
* **Git e GitHub** – utilizados para salvar e acompanhar as alterações do projeto.

---

## 📂 Estrutura do projeto

```text
AppContador/
│
├── app/
│   ├── build.gradle.kts
│   │
│   └── src/
│       └── main/
│           ├── AndroidManifest.xml
│           │
│           └── java/
│               └── com/
│                   └── example/
│                       └── appcontador/
│                           ├── MainActivity.kt
│                           └── ContadorScreen.kt
│
├── build.gradle.kts
├── gradle.properties
├── settings.gradle.kts
└── README.md
```

---

## 📄 Principais arquivos

### `MainActivity.kt`

É o ponto de entrada do aplicativo.

É nele que a aplicação é iniciada e onde a `ContadorScreen()` é chamada para aparecer na tela.

Também foi utilizado o `MaterialTheme` para trabalhar com o tema do aplicativo.

### `ContadorScreen.kt`

É a tela principal do projeto.

A interface foi criada utilizando `@Composable` e Jetpack Compose.

O contador é criado com:

```kotlin
var contador by remember {
    mutableStateOf(0)
}
```

O valor inicial é `0`.

O `mutableStateOf` permite alterar o valor do contador e o `remember` mantém esse estado durante as recomposições da tela.

Quando o botão é clicado, é utilizado:

```kotlin
contador++
```

Assim, o valor aumenta em 1.

### `build.gradle.kts`

Contém configurações importantes do aplicativo, como:

* versão do SDK;
* versão mínima do Android;
* versão de destino;
* plugins;
* dependências utilizadas no projeto.

Também são configuradas as bibliotecas utilizadas pelo Jetpack Compose e Material 3.

### `settings.gradle.kts`

É responsável por configurações gerais do projeto e pela definição do módulo `app`.

### `gradle.properties`

Contém propriedades utilizadas pelo Gradle e pelo projeto Android.

### `AndroidManifest.xml`

É um arquivo importante do aplicativo Android.

Nele é definida a `MainActivity` e qual Activity deve ser iniciada quando o aplicativo é aberto.

---

## 🎨 Interface

A interface foi criada utilizando **Jetpack Compose**.

Foi utilizado um `Column` para organizar os elementos verticalmente.

A tela possui:

* um texto mostrando o valor atual do contador;
* um espaço entre os elementos;
* um botão para adicionar 1 ao contador.

As cores são utilizadas através do:

```kotlin
MaterialTheme.colorScheme
```

Dessa forma, o projeto utiliza as cores definidas pelo tema do Material 3.

---

## 🧠 O que eu aprendi

Durante o desenvolvimento, pude praticar alguns conceitos importantes de Kotlin e Jetpack Compose:

* criação de funções `@Composable`;
* utilização de `remember`;
* utilização de `mutableStateOf`;
* alteração de valores através de eventos de botão;
* organização dos arquivos de um projeto Android;
* utilização do `MaterialTheme`;
* utilização do Git e GitHub para controlar as alterações.

---

## 🚀 Funcionamento

Ao iniciar o aplicativo, o contador aparece com o valor:

**0**

Ao clicar no botão **Adicionar**, o valor aumenta em 1.

```text
0 → 1 → 2 → 3 → 4 → 5...
```

Cada clique adiciona **1** ao valor atual.

---

## 📌 Considerações finais

Este projeto foi desenvolvido como uma forma de praticar os primeiros conceitos de desenvolvimento Android com Kotlin e Jetpack Compose.

Mesmo sendo um aplicativo simples, ele ajudou a entender melhor como funciona o estado de uma interface e como uma ação realizada pelo usuário pode alterar o conteúdo mostrado na tela.

O projeto também foi organizado utilizando Git e GitHub, permitindo acompanhar as alterações realizadas durante o desenvolvimento.

---

**👩‍💻 Desenvolvido por Beatriz Gonçalves de Souza**
