<p align="center">
	<img src="https://www.chatwoot.com/docs/img/logo.png" alt="Chatwoot-logo" width="100" />	
	<p align="center">O Chatwoot oferece todas as ferramentas para gerenciar conversas, construir relacionamentos e encantar seus clientes em um só lugar.</p>
</p>

<p align="left">
	<img src="https://whatsapp.com/favicon.ico" alt="WhatsAPP-logo" width="32" />
	<span>Grupo WhatsaAPP: </span>
	<a href="https://chat.whatsapp.com/CLKge3hmHmmBcIL04mBzmT" target="_blank">Grupo</a>
</p>

<hr />
<hr />

**Como adicionar SMTP do Gmail no Chatwoot**

Primeiro você vai precisar criar uma senha única de aplicativo na sua conta Google

Acesse sua conta Google

Vá até o menu “Segurança”

<img src="https://github.com/cwmkt/smtpgmail/blob/main/imagens/Untitled.png" alt="Chatwoot-logo" width="1000" />

Sua conta precisa ter a verificação de duas etapas ativada para fazer esse processo, se não tiver a verificação ativada, siga os passos para que possa ativar, antes de continuar.

Navegue até a opção  “Verificação em duas etapas”

<img src="https://github.com/cwmkt/smtpgmail/blob/main/imagens/Untitled%20(1).png" width="1000" />

Desça até “Senhas de app”

<img src="https://github.com/cwmkt/smtpgmail/blob/main/imagens/Untitled%20(2).png" width="1000" />

Em “Selecionar app” escolha a opção “Outro(nome personalizado)” defina um nome e gere sua senha 

<img src="https://github.com/cwmkt/smtpgmail/blob/main/imagens/Untitled%20(3).png" width="1000" />

Salve a senha em um lugar seguro, ela só é mostrada uma vez

Pronto sua senha foi criada

Agora no terminal dentro do servidor com a sua instalação use

```bash
sudo nano /home/chatwoot/chatwoot/.env
```

<img src="https://github.com/cwmkt/smtpgmail/blob/main/imagens/env-smtp-gmail.png" width="1000" />

Sai e salve o arquivo.

Reinicie seu Chatwoot

```bash
systemctl daemon-reload && systemctl restart chatwoot.target
```

Por último pra validar se tudo ocorreu corretamente, só seguir o guia de [Validação de SMTP] (https://github.com/cwmkt/testsmtp)
<hr />
<hr />
