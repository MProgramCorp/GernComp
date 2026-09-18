# GernComp

GernComp é um software utilitário desenvolvido pela **MProgram Corp.** com o intuito de facilitar a manutenção completa do computador, fornecendo ferramentas de limpeza profunda de disco, otimização de armazenamento (TRIM e Defrag), diagnósticos de rede e atalhos rápidos para ferramentas essenciais do Windows, tudo em uma interface gráfica moderna e responsiva.

---

## Pré-requisitos

- **Sistema Operacional**: Windows 10 ou Windows 11 (64-bit recomendados). (Obs: Em outras versões do Windows, o GernComp não foi testado!)
- **Permissões**: O aplicativo solicita automaticamente privilégios de Administrador (UAC) para executar tarefas de manutenção de baixo nível do sistema.

O GernComp é um executável nativo em C++20 sem dependências externas pesadas, pronto para uso imediato sem necessidade de instalador.

---

## Funcionalidades

### Limpeza e Espaço em Disco
- **Esvaziar a Lixeira**: Libere espaço removendo permanentemente os itens da lixeira de todas as unidades.
- **Limpar Temp (Windows)**: Exclua arquivos temporários acumulados pelo sistema operacional em `C:\Windows\Temp`.
- **Limpar Temp (Local)**: Limpe os arquivos temporários do usuário corrente em `%TEMP%`.
- **Limpar Prefetch (Windows)**: Exclua arquivos de prefetch do Windows para renovar o cache de execução.

### Armazenamento e Backup
- **Escanear Disco (CHKDSK)**: Realize varreduras profundas em busca de setores defeituosos ou erros no sistema de arquivos.
- **Otimizar Disco (TRIM / Defrag)**: Manutenção inteligente de armazenamento — envio de comando nativo **TRIM** em SSDs para preservar o desempenho e prolongar sua vida útil, e desfragmentação completa de blocos em discos rígidos magnéticos (HDDs).
- **Fazer Backup**: Crie cópias de segurança confiáveis de pastas essenciais para prevenir perdas de dados.
- **Criar Pasta**: Crie rapidamente diretórios e estruturas de pastas organizadas para uso diário.

### Rede e Conectividade
- **Redefinir Winsock**: Restaura o catálogo do Winsock, solucionando problemas críticos de conexão e protocolos corrompidos.
- **Limpar Cache DNS**: Esvazia o cache do resolvedor DNS, corrigindo falhas de navegação e redirecionamentos.
- **Renovar Endereço IP**: Libera e renova concessões DHCP (`ipconfig /release` e `/renew`) em segundo plano para sanar conflitos de IP.
- **Testar Conectividade (Ping)**: Diagnóstico ICMP em tempo real que calcula a latência mínima, média e máxima (ms) e estabilidade de rota com servidores DNS globais.

### Atalhos Administrativos
- **Abrir CMD**: Abre prompt de comando instantâneo com privilégios de Administrador.
- **Abrir Limpeza de Disco**: Inicia o utilitário nativo de limpeza de disco do Windows (`cleanmgr.exe`).
- **Abrir MRT**: Executa a Ferramenta de Remoção de Software Mal-intencionado da Microsoft.
- **Abrir Serviços**: Acessa diretamente o console de gerenciamento de serviços do Windows (`services.msc`).

---

## Como usar

1. Faça o download do [GernComp v3.2.0](https://github.com/MProgramCorp/GernComp/releases/tag/v3.2.0) (versão mais recente).
2. Execute o arquivo `GernComp.exe` (as permissões administrativas serão solicitadas automaticamente via UAC).
3. Selecione a ferramenta desejada no menu lateral ou na visão geral do sistema.
4. Acompanhe a barra de status e o progresso em tempo real até a conclusão da tarefa.

---

## Contribuição

Contribuições para o projeto são sempre bem-vindas! Se você tiver alguma sugestão, melhoria ou encontrar algum problema:
1. Abra uma **Issue** relatando o caso ou propondo uma nova ferramenta.
2. Envie um **Pull Request** com suas alterações.

---

## Contato

- **Suporte**: [suporte@mprogram.com.br](mailto:suporte@mprogram.com.br)
- **Sugestões e Contato Geral**: [contato@mprogram.com.br](mailto:contato@mprogram.com.br)
- **Organização GitHub**: [MProgramCorp](https://github.com/MProgramCorp)

---

## Licença

Veja o arquivo [LICENSE.md](LICENSE.md) para os termos de uso do software.

## Notas de Lançamento

Veja o arquivo [RELEASES.md](RELEASES.md) para o histórico completo de versões e notas de lançamento do GernComp.

---

Agradecemos pelo seu apoio contínuo ao **GernComp**. Estamos comprometidos em oferecer a melhor experiência possível. Entre em contato conosco para sugestões ou feedback.
