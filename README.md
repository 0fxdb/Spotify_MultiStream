<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Spotify Multi-Stream</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
            color: #333;
            margin: 40px;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #1DB954;
        }
        h2 {
            color: #333;
        }
        pre {
            background-color: #f0f0f0;
            padding: 10px;
            border-radius: 5px;
            overflow: auto;
        }
        code {
            font-family: "Courier New", Courier, monospace;
            background-color: #eee;
            padding: 2px 4px;
            border-radius: 4px;
        }
    </style>
</head>
<body>

    <h1>🎵 Spotify Multi-Stream</h1>
    <p>Um utilitário para gerenciar múltiplas instâncias de streams do Spotify. Siga as instruções abaixo para configurar e usar o Spotify Multi-Stream e o Spotify Checker.</p>

    <h2>⚙️ Pré-requisitos</h2>
    <ol>
        <li><strong>Instalar o SocksCap:</strong> Baixe e instale o SocksCap para gerenciar o túnelamento através de um proxy.</li>
        <li><strong>Configurar o Proxyserver:</strong> No SocksCap, configure um servidor proxy que será utilizado para as conexões.</li>
        <li><strong>Adicionar listen.exe ao SocksCap:</strong> No SocksCap, adicione o <code>listen.exe</code> como um executável que deve ser tunelado.</li>
        <li><strong>Criar atalho para o proxer:</strong> Crie um atalho na área de trabalho para o <code>listen.exe</code>, renomeie o atalho para <strong>proxer</strong> e mova para a pasta <em>Spotify Multi-Stream</em>.</li>
    </ol>

    <h2>🚀 Como Usar</h2>
    
    <h3>Spotify Checker</h3>
    <p>O Spotify Checker verifica as contas de Spotify contidas no arquivo fornecido.</p>
    <h4>Para executar:</h4>
    <pre><code>spotify_checker.exe $filename $threads</code></pre>
    <h4>Exemplo:</h4>
    <pre><code>spotify_checker.exe db.txt 5</code></pre>

    <ul>
        <li><strong>$filename:</strong> O arquivo contendo as contas (ex: <code>db.txt</code>).</li>
        <li><strong>$threads:</strong> O número de threads a serem usadas (ex: <code>5</code>).</li>
    </ul>

    <h3>Multi-Stream</h3>
    <p>O Multi-Stream permite rodar múltiplas instâncias de Spotify com o link da música que deseja tocar.</p>
    <h4>Para executar:</h4>
    <pre><code>multi_stream.exe $filename $threads $music_link</code></pre>
    <h4>Exemplo:</h4>
    <pre><code>multi_stream.exe db.txt 5 https://open.spotify.com/track/37i9dQZF1EIUKszidLI7pb</code></pre>

    <ul>
        <li><strong>$filename:</strong> O arquivo com as contas (ex: <code>db.txt</code>).</li>
        <li><strong>$threads:</strong> O número de threads para realizar o streaming simultâneo (ex: <code>5</code>).</li>
        <li><strong>$music_link:</strong> O link da música no Spotify (ex: <code>https://open.spotify.com/track/37i9dQZF1EIUKszidLI7pb</code>).</li>
    </ul>

    <h2>📁 Estrutura do Projeto</h2>
    <pre><code>Spotify_MultiStream/
├── multi_stream.exe
├── spotify_checker.exe
├── db.txt
├── srcs/
│   ├── configs.json
│   └── logs.txt
└── proxer.lnk
</code></pre>

    <h2>📋 Notas</h2>
    <ul>
        <li>Certifique-se de que o SocksCap está corretamente configurado antes de rodar os executáveis.</li>
        <li>Verifique se o arquivo de contas está no formato adequado antes de rodar o <code>spotify_checker.exe</code> e o <code>multi_stream.exe</code>.</li>
    </ul>

</body>
</html>
