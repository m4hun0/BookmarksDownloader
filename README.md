# 📌 Backup de Bookmarks do X (Twitter)

> Automatize o download dos seus **bookmarks (salvos)** do X (antigo Twitter) utilizando **gallery-dl** e um simples arquivo `.bat` no Windows.

---

## 🚀 O que este projeto faz?

Este projeto fornece um script **`atualizar_bookmarks.bat`** que:

- 📥 Faz o download de todos os seus bookmarks do X
- 🔐 Utiliza seus **cookies de login** para autenticação
- 🗂 Organiza os arquivos por **categoria e autor**
- ⚡ Executa tudo com **duplo clique** no Windows

Ideal para quem deseja manter um **backup local** de imagens, vídeos e mídias salvas.

---

## 📂 Estrutura do projeto

```
📁 backup-bookmarks-x/
 ├── atualizar_bookmarks.bat
 ├── cookies.txt
 └── README.md
```

---

## 🧠 Como funciona o arquivo `.bat`

O script executa o seguinte comando principal:

```bat
gallery-dl --cookies cookies.txt -o directory.format="{category}/{author}" "https://x.com/i/bookmarks"
```

### 🔍 Explicação do comando

| Parte | Função |
|------|-------|
| `gallery-dl` | Ferramenta de download |
| `--cookies cookies.txt` | Autenticação usando cookies |
| `directory.format` | Organiza os arquivos em pastas |
| URL bookmarks | Página de salvos do X |

📁 Exemplo de saída:
```
twitter/
 └── usuario_exemplo/
     ├── imagem.jpg
     └── video.mp4
```

---

## 🍪 Como obter o arquivo `cookies.txt`

Para que o download funcione, é necessário estar **logado na sua conta do X** usando cookies.

### ✅ Método recomendado (mais fácil)

Utilize a extensão do navegador:

### 🔹 **Get cookies.txt LOCALLY**

- 🌐 Disponível para Chrome e Firefox
- 🔒 Exporta cookies **localmente**, sem enviar dados para servidores externos

#### Passo a passo:
1. Instale a extensão **Get cookies.txt LOCALLY**
2. Acesse https://x.com e faça login
3. Clique na extensão
4. Exporte os cookies como `cookies.txt`
5. Coloque o arquivo na mesma pasta do `.bat`

⚠️ **Nunca compartilhe seu `cookies.txt`**

---

## ▶️ Como usar

1. Instale o **gallery-dl**
2. Extraia seus cookies e salve como `cookies.txt`
3. Coloque os arquivos na mesma pasta
4. Dê **duplo clique** em `atualizar_bookmarks.bat`
5. Aguarde o download finalizar

---

## 🛠 Requisitos

- Windows
- Python 3
- gallery-dl  
  👉 https://github.com/mikf/gallery-dl

---

## ⚠️

Este projeto é destinado **exclusivamente para backup pessoal**.

Você é totalmente responsável pelo uso da ferramenta e pelo cumprimento dos termos de uso da plataforma X (Twitter).

---
