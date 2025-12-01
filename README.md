# 🧩 **DiskEditor -- Editor Hexadecimal de Setores de Disco (C# WinForms)**

Um poderoso editor hexadecimal desenvolvido em **C# + Windows Forms**,
capaz de **ler, navegar, editar e gravar setores brutos (raw sectors)**
de discos físicos ou arquivos binários.

Ele exibe dados em **HEX + ASCII**, permite navegação por setor, edição
byte a byte e escrita direta --- um recurso extremamente útil, porém
**potencialmente perigoso**.

**Para Inicializar lembre de executar o Visual Studio como ADMINISTRADOR**

------------------------------------------------------------------------

## ⚠️ **AVISO IMPORTANTE**

> ### ⚠️ **RISCO REAL DE CORRUPÇÃO DE DADOS**
>
> Este software permite **escrita direta em setores físicos do disco**.\
> Uso incorreto pode causar: - Corrupção do Windows\
> - Perda de arquivos\
> - Quebra de partições\
> - Sistema não inicializável
>
> **Use somente com conhecimento técnico.**

------------------------------------------------------------------------

# ✨ **Funcionalidades**

## 🔍 **Leitura & Navegação**

-   Seleção de unidades físicas disponíveis\
-   Leitura setor a setor (**512 bytes**)\
-   Exibição em:
    -   Hexadecimal (16 bytes por linha)
    -   ASCII ao lado\
-   Controles de navegação:
    -   ⬅️ **Setor Anterior**
    -   ➡️ **Próximo Setor**
    -   🎯 **Ir para Offset** (HEX ou decimal)
-   🔎 Busca por padrão hexadecimal (ex: `DEADBEEF`)

------------------------------------------------------------------------

## ✏️ **Edição de Dados**

-   Edição direta dos bytes em HEX\
-   Validação automática da entrada\
-   Atualização em tempo real da coluna ASCII\
-   Status mostra qual byte foi modificado\
-   Escrita direta no arquivo ao salvar

------------------------------------------------------------------------

# 🖥️ **Requisitos**

-   ✔️ Windows\
-   ✔️ Visual Studio 2022\
-   ✔️ .NET SDK **8.0+**\
-   ✔️ Executar o Visual Studio **como Administrador**

------------------------------------------------------------------------

# 📥 **Clonando o Repositório**

``` bash
git clone https://github.com/RianGustavoAtanagildo/DiskEditorFinalVersion.git
```

OU:

1.  Clique no botão **Code → Clone**
2.  Copie o link HTTPS
3.  Abra o Visual Studio → *Clone a repository*
4.  Cole o link

------------------------------------------------------------------------

# ▶️ **Como Usar**

## 📂 **Abrir Arquivo**

1.  Clique em **Open**
2.  Escolha um arquivo binário ou imagem de disco

------------------------------------------------------------------------

## 🧭 **Navegação**

O arquivo é dividido automaticamente em setores de **512 bytes**.

Botões: - **Prev Sector** - **Next Sector**

A barra inferior mostra o setor atual.

------------------------------------------------------------------------

## 🔎 **Busca HEX**

Digite um valor HEX no campo **Find**:

    FF 00 1A
    DEADBEEF
    90 90 90

------------------------------------------------------------------------

## 🎯 **Ir Para Offset**

Aceita **decimal** ou **hexadecimal**:

    512
    0x200

------------------------------------------------------------------------

## 📝 **Editar Bytes**

-   Clique no byte desejado
-   Digite o valor em HEX
-   Confirme
-   Clique em **Save** para gravar no arquivo

------------------------------------------------------------------------

# 🛠️ **Tecnologias Utilizadas**

-   C#\
-   .NET 8\
-   Windows Forms\
-   DataGridView\
-   Manipulação de binários\
-   Acesso RAW ao disco

------------------------------------------------------------------------

# 🎓 **Objetivo Acadêmico**

Este projeto demonstra conceitos fundamentais como: - Como setores
representam blocos reais de armazenamento\
- Exibição de dados *HEX + ASCII*\
- Funcionamento de editores hexadecimais\
- Interação entre software e hardware de discos
