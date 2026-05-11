Claro! Vou montar um **README.md completo e organizado** para sua atividade do Dashboard em Blazor 👇

---

# 📊 Dashboard de Finanças Coletivas — RachaAí

Projeto desenvolvido para a disciplina de **Interação Humano Computador e UX** no **Centro Universitário UNA**, com foco na transformação de wireframes em uma interface funcional utilizando **Blazor (C#/.NET)**.

---

## 🎯 Objetivo

Desenvolver uma página estática chamada `Dashboard.razor` que represente o **Dashboard Principal** do aplicativo **RachaAí**, aplicando os conceitos de:

* ✔ Hierarquia Visual
* ✔ Componentização
* ✔ Clareza na exibição de status do sistema
* ✔ Organização de informações financeiras

---

## 🧠 Conceitos Aplicados

* Estruturação de layout com foco em UX
* Uso de componentes reutilizáveis
* Separação entre Modelo (Model) e Interface
* Representação visual de estados financeiros (positivo/negativo)

---

## 🏗 Estrutura do Projeto

```
RachaAiBlazor/
│
├── Pages/
│   └── Dashboard.razor
│
├── Components/
│   └── GrupoCard.razor
│
├── Models/
│   └── Grupo.cs
│
└── wwwroot/
```

---

## 📌 Funcionalidades Implementadas

### 1️⃣ Cards de Resumo (Stats)

Exibição de três indicadores principais:

* 💰 Total a Receber
* 💸 Total a Pagar
* 📊 Saldo Geral

Os cards utilizam destaque visual para indicar situação positiva (azul/verde) ou negativa (vermelho).

---

### 2️⃣ Lista de Grupos

Renderização dinâmica de grupos utilizando o componente:

```
GrupoCard.razor
```

Exemplos de grupos:

* República
* Churrasco de Domingo
* Viagem
* Projeto da Faculdade

Cada card apresenta:

* Nome do grupo
* Categoria
* Valor pendente
* Indicador visual de status (devo ou recebo)

---

### 3️⃣ Botão de Ação Rápida (FAB)

Botão flutuante destacado para:

```
+ Adicionar Novo Gasto
```

Posicionado estrategicamente para fácil acesso, seguindo boas práticas de UX.

---

## 🗂 Modelo de Dados

Arquivo:

```
Models/Grupo.cs
```

Estrutura:

```csharp
namespace RachaAiBlazor.Models
{
    public class Grupo
    {
        public string Nome { get; set; } = string.Empty;
        public string Categoria { get; set; } = string.Empty;
        public decimal ValorPendente { get; set; }
        public bool NoVermelho { get; set; } // true = devo | false = recebo
    }
}
```

---

## 🎨 Decisões de Design

* Layout limpo e organizado
* Separação clara entre resumo financeiro e grupos ativos
* Uso de cores para indicar estado financeiro
* Componentização para melhor reutilização e manutenção
* Hierarquia visual clara (título → resumo → lista → ação)

---

## 🚀 Tecnologias Utilizadas

* Blazor
* C#
* .NET
* Razor Components
* HTML5
* CSS3

---

## 📚 Aprendizados

Durante o desenvolvimento deste projeto foi possível:

* Aplicar conceitos de UX na prática
* Trabalhar com componentização em Blazor
* Criar modelos de dados organizados
* Desenvolver uma interface focada na experiência do usuário

---

## 👨‍💻 Autor

Fernando Ferreira de Oliveira
Curso: Análise e Desenvolvimento de Sistemas
Centro Universitário UNA

