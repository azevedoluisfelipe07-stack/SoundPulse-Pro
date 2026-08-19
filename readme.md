# 🎵 SoundPulse Pro

**SoundPulse Pro** é um player de áudio desenvolvido em HTML, CSS e JavaScript, com foco em uma interface moderna, biblioteca local e recursos avançados de reprodução.

O projeto funciona diretamente no navegador e permite adicionar arquivos de áudio do dispositivo, organizá-los em uma biblioteca local e reproduzi-los com diversos controles.

## ✨ Funcionalidades

* 🎧 Reprodução de arquivos de áudio locais
* 📚 Biblioteca de músicas armazenada localmente
* 💾 Persistência usando **IndexedDB**
* 📤 Upload de múltiplos arquivos
* 🖱️ Suporte a **arrastar e soltar**
* 🔎 Pesquisa de músicas na biblioteca
* ⏮️ Música anterior
* ▶️ Reproduzir / pausar
* ⏭️ Próxima música
* 🔀 Modo aleatório
* 🔁 Modo repetir
* 🔊 Controle de volume
* 🔇 Silenciar áudio
* ⏩ Controle de velocidade de reprodução
* 🎨 Capas personalizadas para cada música
* 🖼️ Catálogo de capas predefinidas
* 📁 Upload de uma imagem própria como capa
* 🎚️ Equalizador de 3 bandas

  * Graves
  * Médios
  * Agudos
* 📊 Visualizador de áudio animado
* 🪟 Modo **Picture-in-Picture (PiP)**
* 🖥️ PiP nativo do navegador quando disponível
* 📌 Mini-player flutuante como alternativa ao PiP nativo
* 🎮 Controles de reprodução no mini-player
* 📱 Interface responsiva
* 🎵 Integração com **Media Session API** para controles de mídia do navegador/sistema

A biblioteca salva os arquivos enviados diretamente no armazenamento local através do IndexedDB.

## 🎨 Interface

O SoundPulse Pro utiliza uma interface escura com estilo moderno, painéis translúcidos e detalhes em verde e roxo.

A interface é dividida principalmente em:

### Player principal

Exibe:

* Capa da música
* Título
* Artista
* Visualizador de áudio
* Botão PiP
* Favoritos

### Biblioteca

Permite visualizar, pesquisar, selecionar, alterar a capa e excluir músicas.

### Player inferior

Possui:

* Aleatório
* Anterior
* Reproduzir / pausar
* Próxima
* Repetir
* Barra de progresso
* Velocidade
* Volume
* Silenciar

## 🪟 Picture-in-Picture

O projeto tenta primeiro utilizar o **Picture-in-Picture nativo do navegador**.

Caso o PiP nativo não esteja disponível ou seja bloqueado, o SoundPulse Pro utiliza um **mini-player flutuante dentro da própria página** como alternativa.

O PiP também possui uma visualização própria com:

* Capa da música
* Título
* Artista
* Barras de áudio animadas

## 🎚️ Equalizador

O equalizador utiliza a Web Audio API e possui três bandas ajustáveis:

| Banda  |           Faixa |
| ------ | --------------: |
| Graves | -12 dB a +12 dB |
| Médios | -12 dB a +12 dB |
| Agudos | -12 dB a +12 dB |

Também existe um botão para restaurar os valores padrão.

## 🖼️ Capas personalizadas

Cada música pode ter sua capa alterada.

É possível:

1. Escolher uma capa predefinida.
2. Enviar uma imagem do dispositivo.

A capa escolhida é salva junto com os dados da música e atualizada no player principal, player inferior e mini-player PiP.

## 🎵 Formatos de áudio

O upload aceita arquivos nos formatos:

* MP3
* WAV
* OGG
* FLAC
* M4A

Os arquivos são tratados como arquivos locais e armazenados na biblioteca do navegador.

## ⚙️ Tecnologias utilizadas

* **HTML5**
* **CSS**
* **JavaScript**
* **Tailwind CSS**
* **Font Awesome**
* **Google Fonts — Inter**
* **IndexedDB**
* **Web Audio API**
* **Canvas API**
* **Picture-in-Picture API**
* **Media Session API**

## 🚀 Como usar

### 1. Baixe o projeto

Tenha o arquivo HTML e os demais arquivos necessários na mesma pasta.

### 2. Abra no navegador

Abra o arquivo `.html` em um navegador moderno.

### 3. Adicione músicas

Clique em **Enviar Áudio** ou arraste os arquivos para a área de upload.

### 4. Reproduza

Selecione uma música na biblioteca e utilize os controles do player.

### 5. Personalize

Você pode alterar a capa, ajustar o equalizador, controlar a velocidade e utilizar o modo PiP.

## 💾 Armazenamento

As músicas e informações da biblioteca são armazenadas localmente usando **IndexedDB**, através do banco `SoundPulseDB`.

Isso significa que a biblioteca é mantida no armazenamento do navegador utilizado pelo projeto.

## 📌 Observações

O funcionamento de alguns recursos, especialmente o **Picture-in-Picture**, depende do suporte e das permissões do navegador. Quando o PiP nativo não está disponível, o projeto possui um mini-player flutuante como fallback.

## 📄 Licença

Este projeto não especifica uma licença no arquivo HTML fornecido.

Caso seja publicado no GitHub, recomenda-se adicionar uma licença apropriada ao repositório.

---

**SoundPulse Pro**
🎵 *Seu player de áudio local com uma experiência mais completa.*
