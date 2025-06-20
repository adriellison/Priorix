# 🧠 Priorix

Sistema de gestão de listas baseado em arquivos Excel, com foco em **reorganização de prioridades** e uma interface visual moderna e intuitiva.

## 🎯 Objetivo

O **Priorix** permite que usuários:

- Façam **upload de arquivos Excel** contendo listas de itens
- **Visualizem e editem** os dados diretamente pela interface web
- **Reorganizem a ordem de prioridade** dos itens através de drag-and-drop
- Exportem os dados com as **prioridades reordenadas**
- Gerenciem múltiplas listas de forma eficiente

## 📁 Estrutura esperada do Excel

A planilha deve conter as seguintes colunas:

| Campo      | Descrição                                  |
| ---------- | ------------------------------------------ |
| ID         | Identificador único do item                |
| Nome       | Nome do item                               |
| Descrição  | Informações adicionais (opcional)          |
| Valor      | Valor estimado                             |
| Imagem     | Caminho da imagem (URL ou nome de arquivo) |
| Prioridade | Número indicando a ordem de compra         |

## 💻 Tecnologias

- **Frontend:** React ou Angular + TailwindCSS
- **Backend:** .NET 8 Web API
- **Base de dados:** Inicialmente não necessário (Excel como fonte principal)
- **Upload/Download:** via API integrada

## 🔁 Lógica de Reordenação

Quando um item é movido ou editado:

1. Sua **prioridade é atualizada**
2. Os itens ao redor são **reordenados automaticamente**
3. O Excel final reflete essa nova ordem

## 🚀 Funcionalidades (MVP)

- [x] Upload de Excel
- [x] Exibição dos itens na interface
- [x] Edição inline de itens (valor, nome, etc.)
- [ ] Drag-and-drop para alterar ordem
- [ ] Download do Excel reorganizado
- [ ] Upload de imagens associadas (opcional)

## 📦 Gerenciamento de Arquivos Excel

O **Priorix** permite:

- 📥 **Importar arquivos Excel** com dados de listas
- 📤 **Exportar listas atualizadas** com nova ordenação de prioridades
- 💾 **Salvar como novo arquivo**, preservando versões anteriores
- 📂 **Escolher arquivos existentes** para abrir diretamente no app
- 🗂️ **Trabalhar com uma pasta padrão**, localizada em `Documentos/Priorix/`
- 🔧 **Alterar a pasta padrão** para outro local personalizado

## 🗂️ Estrutura sugerida do projeto

```ascii
priorix/
│
├── backend/
│   └── ... (.NET API)
│
├── frontend/
│   └── ... (React ou Angular)
│
├── assets/
│   └── exemplo.xlsx
│
└── README.md
```

## 📜 Licença

Este projeto ainda não possui uma licença oficial. Recomenda-se o uso da [MIT License](https://opensource.org/licenses/MIT) para projetos open-source.

---

> Projeto criado por Adriellison Ferreira para automação e organização de listas em Excel.
