# Releases

## [Versão 3.2.0](https://github.com/MProgramCorp/GernComp/releases/tag/v3.2.0)
*Versão mais recente do GernComp*

### Motor Gráfico e Desempenho

- **Migração para DirectX 11 Nativo**: Substituição completa do pipeline gráfico pelo Direct3D 11 moderno com suporte a fallback automático de renderização via software (WARP), garantindo estabilidade máxima em qualquer hardware.
- **Eficiência Energética e Redução a 0% de CPU/GPU**: Suspensão inteligente dos ciclos de renderização ao minimizar a janela, zerando o consumo em segundo plano.
- **Motor de Limpeza Otimizado**: Varredura de arquivos 2x a 3x mais rápida via cache nativo de atributos do C++20 e remoção automática do atributo de somente-leitura em temporários travados.

### Melhorias de Interface (UI/UX)

- **Painel de Rede em Grade 2x2**: Reorganização equilibrada das ferramentas de conectividade em cards simétricos e intuitivos.
- **Padronização Visual Escura (#101116)**: Interface moderna e consistente em todos os módulos, com spinners animados `[ | ] [ / ] [ - ] [ \ ]`.
- **Seletor de Pastas Moderno**: Integração da API COM moderna `IFileOpenDialog` (`FOS_PICKFOLDERS`) substituindo caixas de diálogo legadas.

### Novos Recursos e Segurança

- **Renovação de Configuração IP**: Novo módulo assíncrono para liberar e renovar concessões de endereçamento de rede (`ipconfig /release` e `ipconfig /renew`) com status em tempo real.
- **Teste de Conexão e Latência (Ping)**: Diagnóstico ICMP integrado de alta precisão para teste rápido de estabilidade e tempo de resposta com servidores globais.
- **Otimização Inteligente de Armazenamento**: Módulo com detecção automática do tipo de mídia, aplicando comando TRIM nativo (`defrag /L`) em SSDs e desfragmentação (`defrag /U /V`) em HDDs convencionais.

## Funcionalidades:

- **Esvaziar a Lixeira**: Libere espaço removendo permanentemente os itens da lixeira.
- **Limpar Temp (Windows)**: Remova arquivos temporários do Windows.
- **Limpar Temp (Local)**: Limpe arquivos temporários da pasta local.
- **Limpar Prefetch (Windows)**: Exclua os arquivos de prefetch do Windows.
- **Escanear Disco**: Realize varreduras em busca de erros ou problemas em um disco selecionado.
- **Otimizar Disco (TRIM / Defrag)**: Envie comandos TRIM para preservar SSDs ou desfragmente discos rígidos magnéticos (HDDs).
- **Fazer Backup**: Crie uma cópia de segurança das suas pastas mais importantes para evitar a perda de dados.
- **Criar Pasta**: Adicione novas pastas onde desejar para uma organização personalizada.
- **Abrir CMD**: Abra uma janela de comando para executar comandos ou scripts como Administrador.
- **Abrir Limpeza de Disco**: Abra o programa Limpeza de Disco do próprio Windows para executar uma limpeza.
- **Abrir MRT**: Abra o programa MRT do próprio Windows para executar uma remoção de software malicioso.
- **Abrir Serviços**: Abra o programa Serviços do próprio Windows para modificar os serviços do seu computador.
- **Redefinir Winsock**: Redefinição do Winsock, ajudando com problemas gerais de rede.
- **Limpar Cache DNS**: Limpeza do cache DNS, resolvendo problemas de conectividade.
- **Renovar Endereço IP**: Libere e renove concessões DHCP para resolver conflitos de IP e quedas de conexão.
- **Testar Conectividade (Ping)**: Meça a latência em milissegundos e a estabilidade da internet em tempo real via ICMP.

Agradecemos pelo seu apoio contínuo ao GernComp. Sua opinião é fundamental para nós. Se você tiver alguma dúvida, sugestão ou feedback, entre em contato conosco. Estamos empenhados em proporcionar a melhor experiência possível aos nossos usuários.

---

## [Versão 3.1.0](https://github.com/MProgramCorp/GernComp/releases/tag/v3.1.0)

### Melhorias de Interface (UI/UX)
- Barra de Título Contínua e Arredondamento Nativo: Integração com a API DWM do Windows 11 para cantos arredondados suaves e barra de título contínua de ponta a ponta com botões vetorizados de minimizar e fechar.
- Correção Ortográfica e Tipografia: Ajuste de textos, títulos centralizados e integração das fontes Segoe UI / Segoe UI Semibold.

### Novos Recursos e Segurança
- Validação de Versão Online Assíncrona: Sistema integrado em segundo plano via std::jthread e WinINet que consulta a API do GitHub (MProgramCorp/GernComp) sem travar a interface.
- Popup de Atualização Flutuante (Toast): Notificação translúcida moderna no canto inferior direito informando sobre novas versões disponíveis, com botões para download direto no GitHub ou adiar.

## Funcionalidades:
- Esvaziar a Lixeira: Libere espaço removendo permanentemente os itens da lixeira.
- Limpar Temp (Windows): Remova arquivos temporários do Windows.
- Limpar Temp (Local): Limpe arquivos temporários da pasta local.
- Limpar Prefetch (Windows): Exclua os arquivos de prefetch do Windows.
- Escanear Disco: Realize varreduras em busca de erros ou problemas em um disco selecionado.
- Fazer Backup: Crie uma cópia de segurança das suas pastas mais importantes para evitar a perda de dados.
- Criar Pasta: Adicione novas pastas onde desejar para uma organização personalizada.
- Abrir CMD: Abra uma janela de comando para executar comandos ou scripts como Administrador.
- Abrir Limpeza de Disco: Abra o programa Limpeza de Disco do próprio Windows para executar uma limpeza.
- Abrir MRT: Abra o programa MRT do próprio Windows para executar uma remoção de software malicioso.
- Abrir Serviços: Abra o programa Serviços do próprio Windows para modificar os serviços do seu computador.
- Redefinir Winsock: Redefinição do Winsock, ajudando com problemas gerais de rede.
- Limpar Cache DNS: Limpeza do cache DNS, resolvendo problemas de conectividade.

Agradecemos pelo seu apoio contínuo ao GernComp. Sua opinião é fundamental para nós. Se você tiver alguma dúvida, sugestão ou feedback, entre em contato conosco. Estamos empenhados em proporcionar a melhor experiência possível aos nossos usuários.

---

## [Versão 3.0.0](https://github.com/MProgramCorp/GernComp/releases/tag/v3.0.0)

### Reformulação Completa do Código-Fonte e Interface Gráfica
- Reformulação completa do código-fonte de C/WinGUI para C++20 utilizando Dear ImGui e DirectX 9.
- Nova interface gráfica moderna estilo Fluent Dark inspirada no Windows 11.
- Adicionada elevação automática de permissões de Administrador (UAC) ao executar o programa.
- Execução de tarefas em segundo plano com suporte a multithreading (`std::jthread`), evitando o travamento da interface.
- Remoção total de dependências do `system()`, utilizando APIs nativas do Windows para maior desempenho e estabilidade.
  
## Funcionalidades:
- Esvaziar a Lixeira: Libere espaço removendo permanentemente os itens da lixeira.
- Limpar Temp (Windows): Remova arquivos temporários do Windows.
- Limpar Temp (Local): Limpe arquivos temporários da pasta local.
- Limpar Prefetch (Windows): Exclua os arquivos de prefetch do Windows.
- Escanear Disco: Realize varreduras em busca de erros ou problemas em um disco selecionado.
- Fazer Backup: Crie uma cópia de segurança das suas pastas mais importantes para evitar a perda de dados.
- Criar Pasta: Adicione novas pastas onde desejar para uma organização personalizada.
- Abrir CMD: Abra uma janela de comando para executar comandos ou scripts como Administrador.
- Abrir Limpeza de Disco: Abra o programa Limpeza de Disco do próprio Windows para executar uma limpeza.
- Abrir MRT: Abra o programa MRT do próprio Windows para executar uma remoção de software malicioso.
- Abrir Serviços: Abra o programa Serviços do próprio Windows para modificar os serviços do seu computador.
- Redefinir Winsock: Redefinição do Winsock, ajudando com problemas gerais de rede.
- Limpar Cache DNS: Limpeza do cache DNS, resolvendo problemas de conectividade.
  
Agradecemos pelo seu apoio contínuo ao GernComp. Sua opinião é fundamental para nós. Se você tiver alguma dúvida, sugestão ou feedback, entre em contato conosco. Estamos empenhados em proporcionar a melhor experiência possível aos nossos usuários.

---

## [Versão 2.2.0](https://github.com/MProgramCorp/GernComp/releases/tag/v2.2.0)

### Melhorias do Menu Principal
- Reorganização do menu principal para uma experiência de uso mais intuitiva.
- Nova opção "Rede" agrupa algumas funções de limpeza do wifi para fácil acesso do usuário.
- Novo atalho denominado "Serviços", está agrupado no menu "Atalhos".

### Novas funcionalidades Adicionadas
- Serviços: Agora você pode abrir o programa services.msc do próprio Windows diretamente pelo GernComp, no menu "Atalhos".
- Redefinir Winsock: Agora você pode fazer a redefinição do Winsock (pode ajudar com problemas gerais de rede) diretamente do GernComp, no menu "Rede".
- Limpar Cache DNS: Agora você pode fazer a limpeza de cache do DNS (pode ajudar a resolver problemas de conectividade) diretamente do GernComp, no menu "Rede".

## Funcionalidades:
- Esvaziar a Lixeira: Libere espaço removendo permanentemente os itens da lixeira.
- Limpar Temp (Windows): Remova arquivos temporários do Windows.
- Limpar Temp (Local): Limpe arquivos temporários da pasta local.
- Limpar Prefetch (Windows): Exclua os arquivos de prefetch do Windows.
- Escanear Disco: Realize varreduras em busca de erros ou problemas em um disco selecionado.
- Fazer Backup: Crie uma cópia de segurança das suas pastas mais importantes para evitar a perda de dados.
- Criar Pasta: Adicione novas pastas onde desejar para uma organização personalizada.
- Abrir CMD: Abra uma janela de comando para executar comandos ou scripts.
- Abrir Limpeza de Disco: Abra o programa Limpeza de Disco do próprio Windows para executar uma limpeza.
- Abrir MRT: Abra o programa MRT do próprio Windows para executar uma remoção de software malicioso.
- Abrir Serviços: Abra o programa Serviços do próprio Windows para modificar os serviços do seu computador.
- Redefinir Winsock: Redefinição do Winsock, ajudando com problemas gerais de rede.
- Limpar Cache DNS: Limpeza do cache DNS, resolvendo problemas de conectividade.

Agradecemos pelo seu apoio contínuo ao GernComp. Sua opinião é fundamental para nós. Se você tiver alguma dúvida, sugestão ou feedback, entre em contato conosco. Estamos empenhados em proporcionar a melhor experiência possível aos nossos usuários.

---

## [Versão 2.1.0](https://github.com/MProgramCorp/GernComp/releases/tag/v2.1.0)

### Melhorias do Menu Principal
- Reorganização do menu principal para uma experiência de uso mais intuitiva.
- Nova opção "Atalhos" agrupa alguns atalhos de aplicativos para fácil acesso do usuário.
- A opção abrir CMD agora está agrupada no novo menu "Atalhos".
- Nova opção para limpeza da pasta "Recent", está agrupada no menu "Limpeza".

### Novas funcionalidades Adicionadas
- Limpeza de Disco: Agora você pode abrir o programa Limpeza de Disco do próprio Windows diretamente pelo GernComp, no menu "Atalhos".
- MRT: Agora você pode abrir o programa MRT do próprio Windows diretamente pelo GernComp, no menu "Atalhos".
- Criar Pasta em Sequência: Agora você pode criar várias pastas em sequência, sem precisar reiniciar a funcionalidade.

## Funcionalidades:
- Esvaziar a Lixeira: Libere espaço removendo permanentemente os itens da lixeira.
- Limpar Temp (Windows): Remova arquivos temporários do Windows.
- Limpar Temp (Local): Limpe arquivos temporários da pasta local.
- Limpar Prefetch (Windows): Exclua os arquivos de prefetch do Windows.
- Escanear Disco: Realize varreduras em busca de erros ou problemas em um disco selecionado.
- Fazer Backup: Crie uma cópia de segurança das suas pastas mais importantes para evitar a perda de dados.
- Criar Pasta: Adicione novas pastas onde desejar para uma organização personalizada.
- Abrir CMD: Abra uma janela de comando para executar comandos ou scripts.
- Abrir Limpeza de Disco: Abra o programa Limpeza de Disco do próprio Windows para executar uma limpeza.
- Abrir MRT: Abra o programa MRT do próprio Windows para executar uma remoção de software malicioso.

Agradecemos pelo seu apoio contínuo ao GernComp. Sua opinião é fundamental para nós. Se você tiver alguma dúvida, sugestão ou feedback, entre em contato conosco. Estamos empenhados em proporcionar a melhor experiência possível aos nossos usuários.

---

## [Versão 2.0.1](https://github.com/MProgramCorp/GernComp/releases/tag/v2.0.1)

### Melhorias do Menu Principal
- Reorganização do menu principal para uma experiência de uso mais intuitiva.
- A opção de limpeza de arquivos temporários agora está agrupada no novo menu "Limpeza".

### Novas funcionalidades Adicionadas
- Criar Pasta Avançada: Agora você pode criar pastas em qualquer local do seu computador para uma organização mais flexível.
- Backup Personalizado: Faça backups de qualquer parte do seu computador para outra, garantindo a segurança dos seus dados.

## Funcionalidades:
- Esvaziar a Lixeira: Libere espaço removendo permanentemente os itens da lixeira.
- Limpar Temp (Windows): Remova arquivos temporários do Windows.
- Limpar Temp (Local): Limpe arquivos temporários da pasta local.
- Limpar Prefetch (Windows): Exclua os arquivos de prefetch do Windows.
- Escanear Disco: Realize varreduras em busca de erros ou problemas em um disco selecionado.
- Fazer Backup: Crie uma cópia de segurança das suas pastas mais importantes para evitar a perda de dados.
- Criar Pasta: Adicione novas pastas onde desejar para uma organização personalizada.
- Abrir CMD: Abra uma janela de comando para executar comandos ou scripts.

Agradecemos pelo seu apoio contínuo ao GernComp. Sua opinião é fundamental para nós. Se você tiver alguma dúvida, sugestão ou feedback, entre em contato conosco. Estamos empenhados em proporcionar a melhor experiência possível aos nossos usuários.

---

## [Versão 2.0.0](https://github.com/MProgramCorp/GernComp/releases/tag/v2.0.0)

### Novo código fonte
- Houve a reformulação do código fonte, agora sendo escrito em C.

### Implementação de várias melhorias e novas funcionalidades
- Nova interface gráfica, simples e rápida.

### Correção de bugs e problemas relatados pelos usuários
- A função de esvaziamento da lixeira foi corrigida.

## Funcionalidades:
- Esvaziar a Lixeira: Libere espaço em disco removendo permanentemente os itens da lixeira.
- Limpar Temp (Windows): Remova arquivos temporários do Windows.
- Limpar Temp (Local): Limpe arquivos temporários da pasta local.
- Limpar Prefetch (Windows): Exclua os arquivos de prefetch do Windows.
- Escanear Disco: Realize uma varredura completa em um disco selecionado em busca de erros ou problemas.
- Fazer Backup (Documentos): Crie uma cópia de segurança dos seus documentos importantes para evitar a perda de dados.
- Criar Pasta: Crie facilmente novas pastas na área de trabalho.
- Abrir CMD: Abra uma janela de comando para executar comandos ou scripts.

Agradecemos pelo seu apoio contínuo ao GernComp. Se você tiver alguma dúvida, sugestão ou feedback, não hesite em entrar em contato conosco. Estamos comprometidos em oferecer a melhor experiência aos nossos usuários.

---

## [Versão 1.0.1](https://github.com/MProgramCorp/GernComp/releases/tag/v1.0.1)

### Funcionalidades:
- Esvaziar a Lixeira
- Limpar Temp (Win)
- Limpar Temp (Local)
- Limpar Prefetch (Win)
- Escanear Disco
- Fazer Backup (Documentos)
- Criar Pasta
- Abrir CMD

*Observação: Nesta versão, a função de esvaziamento da lixeira ainda não foi corrigida.*

Pedimos desculpas por qualquer inconveniente causado por essa falha e estamos trabalhando para solucionar o problema o mais rápido possível. Planejamos lançar uma versão atualizada em breve, onde a função de esvaziamento da lixeira estará funcionando corretamente.

Agradecemos seu interesse e apoio contínuo ao nosso programa. Se você tiver alguma dúvida ou feedback, não hesite em entrar em contato conosco.

---

## [Versão 1.0.0](https://github.com/MProgramCorp/GernComp/releases/tag/v1.0.0)
*Esta é a versão inicial do GernComp.*

### Funcionalidades:
- Esvaziar a Lixeira
- Limpar Temp (Win)
- Limpar Temp (Local)
- Limpar Prefetch (Win)
- Escanear Disco
- Fazer Backup (Documentos)

*Observação: Nesta versão, a função de esvaziamento da lixeira está passando por problemas de funcionamento e ainda não foi corrigida.*

Pedimos desculpas por qualquer inconveniente causado por essa falha e estamos trabalhando para solucionar o problema o mais rápido possível. Planejamos lançar uma versão atualizada em breve, onde a função de esvaziamento da lixeira estará funcionando corretamente.
