# 🎵 Spotify Multi-Stream

Um utilitário para gerenciar múltiplas instâncias de streams do Spotify. Siga as instruções abaixo para configurar e usar o Spotify Multi-Stream e o Spotify Checker.

## ⚙️ Pré-requisitos

1. **Instalar o SocksCap:** Baixe e instale o SocksCap para gerenciar o túnelamento através de um proxy.
2. **Configurar o Proxyserver:** No SocksCap, configure um servidor proxy que será utilizado para as conexões.
3. **Adicionar `listen.exe` ao SocksCap:** No SocksCap, adicione o `listen.exe` como um executável que deve ser tunelado.
4. **Criar atalho para o `proxer`:** Crie um atalho na área de trabalho para o `listen.exe`, renomeie o atalho para **proxer** e mova para a pasta "Spotify Multi-Stream".

## 🚀 Como Usar

### Spotify Checker

O Spotify Checker verifica as contas de Spotify contidas no arquivo fornecido.

#### Para executar:

```bash
spotify_checker.exe $filename $threads

````

### Spotify Multi Stream

O Spotify Multi Stream strema uma mesma música em todas as contas contidas no arquivo fornecido utilizando multithreading.

#### Para executar:

```bash
multi_stream.exe $filename $threads $link
