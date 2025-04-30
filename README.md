<h1>📊 Monitoramento de Site com Webhook 🚀</h1>

<p>Este projeto tem como objetivo monitorar se um site está no ar e, caso não esteja, enviar uma mensagem de alerta para o <strong>Discord</strong>, <strong>Slack</strong> ou <strong>Telegram</strong> usando Webhooks. O monitoramento é feito a cada 1 minuto.</p>

<h2>📋 Etapa Inicial - Visão Geral das Etapas</h2>
<p>O processo será dividido nas seguintes etapas:</p>
<ol>
    <li><strong>Etapa 1:</strong> Montar o ambiente local (VM ou Subsystems).</li>
    <li><strong>Etapa 2:</strong> Subir o servidor Nginx.</li>
    <li><strong>Etapa 2.5:</strong> Montar um site simples.</li>
    <li><strong>Etapa 3:</strong> Criar o script de verificação de site e integração com Webhooks.</li>
    <li><strong>Etapa 3.5:</strong> Configurar log para monitoramento com informações de status.</li>
    <li><strong>Etapa 4:</strong> Testar a integração do Webhook.</li>
    <li><strong>Etapa 5:</strong> Agendar a execução do script a cada 1 minuto.</li>
</ol>

<h2>🚀 Etapa 1 - Montar Ambiente Local (VM ou Subsystems)</h2>
<ol>
    <li><strong>Instalar o Ubuntu pela Microsoft Store</strong>:
        <p>Abra a Microsoft Store, busque por "Ubuntu" e instale a versão desejada.</p>
    </li>
    <li><strong>Instalar o WSL (Windows Subsystem for Linux)</strong>:
        <pre>wsl --install -d Ubuntu</pre>
    </li>
    <li><strong>Abrir o Ubuntu no terminal</strong>:
        <pre>wsl </pre>
    </li>
</ol>

<h2>🚀 Etapa 2 - Subir Servidor Nginx</h2>
<ol>
    <li><strong>Instalar o Nginx</strong>:
        <pre>sudo apt-get update</pre>
        <pre>sudo apt-get install nginx</pre>
    </li>
   <li><strong>Após instalar o Nginx</strong>
      <p>Execute o comando <pre>systemctl status nginx</pre> em seu terminal e deve aparecer a seguinte mensagem</p>
      ![image](https://github.com/user-attachments/assets/353a3442-111d-426e-85ca-1fc57adebecb)

    </li>
    <li><strong>Iniciar o Nginx</strong>:
        <pre>sudo systemctl start nginx</pre>
    </li>
    <li><strong>Verificar se o Nginx está funcionando</strong>: Acesse <a href="http://localhost">http://localhost</a> ou o IP da máquina.</li>
</ol>
