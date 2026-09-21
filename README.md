# Criação de um phishing com Kali Linux

Projeto desenvolvido para o desafio **Criação de um Phishing com o Kali Linux**, da Formação Cybersecurity Specialist da [DIO](https://www.dio.me/).

## Sobre o projeto

O objetivo deste laboratório foi compreender, em um ambiente controlado, como campanhas de engenharia social podem reproduzir interfaces conhecidas para induzir o envio de informações. A atividade também reforça a importância de verificar endereços, desconfiar de páginas inesperadas e utilizar autenticação multifator.

> **Uso ético:** todo o procedimento foi realizado em máquina virtual própria, com dados fictícios e exclusivamente para fins educacionais. O projeto não deve ser utilizado contra terceiros ou sistemas sem autorização expressa.

## Objetivos de aprendizagem

- Configurar um laboratório isolado com Kali Linux;
- conhecer o fluxo de criação de páginas de demonstração no Social-Engineer Toolkit;
- entender como formulários podem ser manipulados em ataques de engenharia social;
- registrar evidências e documentar decisões técnicas;
- reconhecer medidas de prevenção contra phishing.

## Ambiente utilizado

- Kali Linux 2026.2 em máquina virtual;
- Oracle VirtualBox;
- Social-Engineer Toolkit (SET) 8.1.3;
- rede local privada do laboratório;
- credenciais fictícias para validação.

## Etapas realizadas

1. Preparação da máquina virtual Kali Linux.
2. Identificação do endereço IP privado do laboratório.
3. Inicialização do SET com privilégios administrativos.
4. Seleção de **Social-Engineering Attacks**.
5. Seleção de **Website Attack Vectors**.
6. Configuração do método demonstrado nas aulas em ambiente controlado.
7. Importação da página de laboratório e execução local.
8. Envio de dados fictícios para confirmar o funcionamento.
9. Registro da evidência e encerramento dos serviços utilizados.

## Resultado

A execução confirmou que o formulário de demonstração recebeu os campos fictícios enviados no laboratório. A captura abaixo registra o resultado ao lado da página do curso.

![Resultado do laboratório de phishing no Kali Linux](./images/resultado-laboratorio.png)

## Problemas encontrados

Durante a atividade, a versão 8.1.3 do SET apresentou uma referência ausente ao arquivo `src/webattack/tabnabbing/source.js`. A instalação também dependia do diretório de execução correto para resolver caminhos relativos. O laboratório foi concluído após restaurar o recurso esperado, corrigir a resolução do caminho e manter os arquivos dentro do ambiente local.

## Como identificar e evitar phishing

- Confira cuidadosamente o domínio antes de informar qualquer dado;
- não acesse páginas sensíveis por links recebidos de forma inesperada;
- utilize um gerenciador de senhas, que ajuda a detectar domínios diferentes;
- ative autenticação multifator;
- nunca reutilize senhas;
- comunique páginas suspeitas à organização responsável.

## Referências

- [Social-Engineer Toolkit](https://github.com/trustedsec/social-engineer-toolkit)
- [Repositório base do desafio](https://github.com/cassiano-dio/cibersecurity-desafio-phishing)
- [Formação Cybersecurity Specialist — DIO](https://web.dio.me/track/formacao-cybersecurity)
- [OWASP: Phishing](https://owasp.org/www-community/attacks/Phishing)

## Autor

Desenvolvido por [2f-developer](https://github.com/2f-developer) como parte da Formação Cybersecurity Specialist da DIO.
