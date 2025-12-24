🔐 Espólio Digital
Sistema de Gestão de Herança Digital e Ativos Post-Mortem.
💻 Sobre o Projeto
O Espólio Digital é uma aplicação web desenvolvida como Projeto Final (M2) para o curso de Análise e Desenvolvimento de Sistemas da UMC.
O sistema soluciona o problema da perda de ativos digitais (redes sociais, criptomoedas, milhas, senhas) após o falecimento do titular. Ele permite que o usuário cadastre seus bens digitais e designe herdeiros. A liberação dos dados sensíveis (senhas) só ocorre mediante um fluxo de segurança que exige o upload e validação da Certidão de Óbito.
🎯 Principais Funcionalidades
	•	Cofre Digital: Cadastro criptografado de logins, senhas e chaves de segurança.
	•	Gestão de Herdeiros: Vínculo de ativos a CPFs específicos.
	•	Upload Seguro: Envio de Certidão de Óbito em PDF para desbloqueio de legado.
	•	Armazenamento Binário: Arquivos salvos diretamente no banco de dados (LONGBLOB) para maior segurança.
	•	Interface Responsiva: Telas construídas com TailwindCSS.
🛠 Tecnologias Utilizadas
	•	Backend: Java (Servlets, JSP, JDBC)
	•	Frontend: HTML5, TailwindCSS
	•	Banco de Dados: MySQL 8.0
	•	Segurança: Criptografia AES-256 (Dados) e SHA-256 (Senhas de Acesso)
	•	IDE: Apache NetBeans
🚀 Como Executar o Projeto
Pré-requisitos
	•	Java JDK 17+
	•	Apache Tomcat 9.0
	•	MySQL Server
Passo a Passo
	1	Clone o repositório: git clone [https://github.com/dibaaloned/Espolio-Digital.git](https://github.com/dibaaloned/Espolio-Digital.git)  
	2	Banco de Dados:
	•	Acesse a pasta /database.
	•	Execute o script script_banco.sql no seu MySQL Workbench para criar o banco espoliodigital.
	3	Configuração:
	•	Abra o projeto no NetBeans.
	•	No arquivo src/java/config/ConectaDB.java, verifique se o usuário e senha do banco correspondem ao seu ambiente local.
	4	Execução:
	•	Execute o projeto (F6). O Tomcat irá iniciar e abrirá a página de login.
🗄️ Modelagem de Dados
O sistema utiliza 4 tabelas principais:
	•	usuario: Titulares e Herdeiros.
	•	herdeiro: Vínculo entre pessoas.
	•	ativodigital: As contas e senhas (criptografadas).
	•	solicitacao_liberacao: Onde ficam os PDFs das certidões.
(Veja o DER completo na pasta /docs)
👥 Autores
	•	Diego Henrique de Oliveira (RGM: 11241102717)
	•	Tiago Kuan Mello Duran Ferreira (RGM: 11241103205)
	•	Nicoly Fernandes Amancio Martineli (RGM: 11241103083)
📄 Licença
Este projeto está sob a licença MIT.
