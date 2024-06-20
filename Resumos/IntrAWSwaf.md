# AWS Well-Architected Framework

## O Que é o AWS Well-Architected Framework?

*O AWS Well-Architected Framework, é um conjunto de práticas recomendadas para projetar e operar sistemas na nuvem AWS. O AWS WAF ajuda você a entender os prós e os contras das decisões que você toma ao criar sistemas na AWS.*

*Usar o AWS Well-Architected Framework traz vários benefícios, tais como:*

- *Aumentar a confiança e a capacidade de tomar decisões arquiteturais informadas;*
- *Melhorar a qualidade e a performance dos sistemas na nuvem;*
- *Reduzir os riscos e os custos associados aos sistemas na nuvem;*
- *Acelerar a inovação e a entrega de valor para os clientes;*
- *linhar os sistemas com as melhores práticas e os padrões da AWS;*

## Os Pilares do AWS Well-Architected Framework

### Excelência Operacional
*O pilar de excelência operacional se concentra na execução e no monitoramento de sistemas e na melhoria contínua de processos e procedimentos.*

- **Automatizar as mudanças**: *usar processos automatizados para aplicar mudanças nos sistemas, reduzindo erros humanos, aumentando a velocidade e a consistência, e facilitando o rastreamento e a reversão de mudanças*
- **Reagir a eventos**: *usar mecanismos de resposta a eventos para acionar ações automatizadas ou notificações quando ocorrem eventos significativos nos sistemas, como falhas, picos de demanda, alterações de configuração, etc.*
- **Definir padrões**: *usar padrões e políticas para estabelecer as expectativas e os requisitos de qualidade dos sistemas, facilitar a comunicação e a colaboração entre as equipes envolvidas no ciclo de vida dos sistemas.*
- **Antecipar falhas**: *usar técnicas de teste e simulação para identificar e eliminar pontos de falha nos sistemas, aumentar a resiliência e a tolerância a falhas dos sistemas.*
- **Aprender com a experiência**: *usar métricas e indicadores para monitorar o desempenho e a saúde dos sistemas, coletar e analisar dados sobre os eventos e as mudanças que ocorrem nos sistemas, gerando aprendizados e ações de melhoria.*

### Segurança
*O pilar de segurança se concentra na proteção de informações e sistemas, incluindo confidencialidade, integridade e disponibilidade de dados, gerenciamento de identidades e acessos, e detecção e resposta a eventos de segurança.*

- **Implementar um forte controle de identidade**: *usar o princípio do menor privilégio para conceder apenas os acessos necessários aos recursos e operações dos sistemas, e usar mecanismos de autenticação e autorização robustos e seguros para validar as identidades e os acessos dos usuários e das aplicações.*
- **Proteger os dados em trânsito e em repouso**: *usar técnicas de criptografia e assinatura para garantir a confidencialidade e a integridade dos dados que são transmitidos ou armazenados nos sistemas, e usar mecanismos de gerenciamento de chaves seguros e confiáveis para proteger as chaves de criptografia.*
- **Aplicar a defesa em profundidade**: *usar múltiplas camadas de segurança para proteger os sistemas contra ataques, incluindo firewalls, grupos de segurança, listas de controle de acesso, detecção e prevenção de intrusão, isolamento de rede, etc.*
- **Automatizar a segurança**: *usar processos automatizados para aplicar as políticas e os padrões de segurança nos sistemas, detectar e responder a eventos de segurança, como tentativas de invasão, violações de dados, vulnerabilidades, etc.*
- **Preparar- incidentes de segurança**: *usar planos e procedimentos para lidar com incidentes de segurança, incluindo comunicação, investigação, recuperação, análise e ações corretivas.*

### Confiabilidade
*O pilar de confiabilidade se concentra na capacidade dos sistemas de executar as funções pretendidas e de se recuperar rapidamente de falhas, atendendo às demandas de mudança e crescimento.*
- **Testar a recuperação**: *usar técnicas de teste e simulação para verificar a capacidade dos sistemas de se recuperar de falhas, medir os tempos e os impactos de recuperação.*
- **Gerenciar alterações**: *usar processos de gerenciamento de mudanças para controlar e monitorar as alterações nos sistemas, avaliar os riscos e os benefícios das alterações.*
- **Lidar com a demanda**: *usar técnicas de escalabilidade e elasticida ajustar a capacidade dos sistemas de acordo com a demanda, evitar a degradação ou a indisponibilidade dos sistemas.*
- **Distribuir os recursos**: *usar técnicas de distribuição e balanceamento de carga para distribuir os recursos dos sistemas entre múltiplas zonas de disponibilidade e regiões, aumentar a disponibilidade e a performance dos sistemas.*
- **Monitorar e alertar**: *usar métricas e indicadores para monitorar o desempenho e a saúde dos sistemas, gerar alertas quando ocorrem anomalias ou falhas nos sistemas*

### Eficiência de Performance
*O pilar de eficiência de performance se concentra na alocação eficaz e otimizada de recursos, incluindo seleção, provisionamento, monitoramento e ajuste de recursos.*

- **Selecionar os recursos certos**: *usar os recursos que melhor atendem aos requisitos funcionais e não funcionais dos sistemas, considerando fatores como tipo, tamanho, capacidade, performance, custo, etc.*
- **Provisionar os recursos de forma eficiente**: *usar técnicas de provisionamento e configuração de recursos para alocar os recursos de forma rápida e consistente, evitar o desperdício ou a subutilização de recursos.*
- **Monitorar e avaliar os recursos**: *usar métricas e indicadores para monitorar o desempenho e a utilização dos recursos, avaliar se os recursos estão atendendo às expectativas e aos objetivos dos sistemas.*
- **Ajustar os recursos de forma dinâmica**: *usar técnicas de ajuste e otimização de recursos para adaptar os recursos às mudanças nas condições e nas demandas dos sistemas, melhorar a performance e a eficiência dos recursos.*


### Otimização de Custos
*O pilar de otimização de custos se concentra na obtenção do melhor retorno sobre o investimento em recursos, incluindo análise, medição, previsão e controle de custos.*

- **Analisar e atribuir os custos**: *usar ferramentas e métodos para analisar e atribuir os custos dos recursos, entender os fatores que influenciam os custos, como uso, performance, qualidade, etc.*
- **Medir e reportar os custos**: *usar ferramentas e métodos para medir e reportar os custos dos recursos, comparar os custos com os orçamentos e os objetivos dos sistemas.*
- **Prever e planejar os custos**: *usar ferramentas e métodos para prever e planejar os custos dos recursos, estimar os cenários e as tendências de custos.*
- **Controlar e otimizar os custos**: *usar ferramentas e métodos para controlar e otimizar os custos dos recursos, aproveitar as oportunidades de redução de custos, como descontos, reservas, modelos de consumo, etc.*

### Sustentabilidade
*Especificamente, o pilar de sustentabilidade se concentra na redução do impacto ambiental dos sistemas na nuvem, incluindo consumo de energia, emissão de carbono, uso de materiais e descarte de resíduos.*

- **Medir o impacto ambiental**: *usar ferramentas e métodos para medir o impacto ambiental dos recursos, entender os fatores que influenciam o impacto, como localização, fonte de energia, eficiência energética, etc.*
- **Reportar o impacto ambiental**: *usar ferramentas e métodos para reportar o impacto ambiental dos recursos, comparar o impacto com as metas e os objetivos de sustentabilidade dos sistemas.*
- **Reduzir o impacto ambiental**: *usar ferramentas e métodos para reduzir o impacto ambiental dos recursos, aproveitar as oportunidades de melhoria de sustentabilidade, como migração para regiões mais verdes, otimização de recursos, uso de serviços gerenciados, etc.*
- **Compensar o impacto ambiental**: *usar ferramentas e métodos para compensar o impacto ambiental dos recursos, apoiar iniciativas de sustentabilidade, como projetos de carbono neutro, programas de reciclagem, doações para ONGs ambientais, etc.*
