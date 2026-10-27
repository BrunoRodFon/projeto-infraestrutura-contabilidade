# Projeto de Infraestrutura de TI — Escritório de Contabilidade

## Sobre o projeto

Este repositório reúne os materiais de um projeto acadêmico de planejamento e simulação da infraestrutura de TI de um escritório de contabilidade com aproximadamente 50 colaboradores.

O projeto contempla o planejamento físico e lógico da rede, a segmentação por VLANs, o endereçamento IP, os serviços de rede, as políticas de controle de acesso e a documentação dos testes realizados no Cisco Packet Tracer.

## Objetivos

- Planejar a infraestrutura física e lógica da rede.
- Organizar os dispositivos e setores por meio de VLANs.
- Definir um plano de endereçamento IP.
- Configurar e validar serviços de rede na simulação, conforme documentado.
- Aplicar políticas de controle de acesso por meio de ACLs.
- Registrar evidências e resultados dos testes.
- Apresentar uma estimativa de materiais e custos para a infraestrutura proposta.

## Tecnologias e ferramentas

- **Cisco Packet Tracer:** simulação da infraestrutura e dos dispositivos de rede.
- **Lucidchart, Microsoft Visio e Canva:** elaboração de diagramas, plantas e materiais visuais.
- **Visual Paradigm:** elaboração do diagrama do rack.

## Estrutura do repositório

```text
projeto-infraestrutura-contabilidade/
├── Documentacao/
│   ├── Projeto-Infraestrutura.pdf
│   ├── Projeto-Infraestrutura.docx
│   ├── planta-fisica.png
│   └── diagrama-rack.png
├── Packet-Tracer/
│   ├── infraestrutura-contabilidade.pkt
│   └── README.md
├── ACLs/
│   ├── ACL-GERENCIAMENTO-RESTRITO/
│   │   ├── ping-gerenciamento.png
│   │   ├── README.md
│   └── ACL-VISITANTES-ISOLAMENTO/
│       ├── ping-visitantes.png
│       ├── README.md
├── Testes/
│   ├── dhcp.png
│   ├── dns-intranet.png
│   ├── conectividade-vlans.png
│   ├── isolamento-visitantes.png
│   └── resultados.md
├── README.md
└── .gitignore
```

## Como consultar o projeto

1. Acesse `Documentacao/` para ler o relatório acadêmico e consultar os diagramas.
2. Abra `Packet-Tracer/infraestrutura-contabilidade.pkt` no Cisco Packet Tracer para visualizar a simulação.
3. Consulte `ACLs/` para conhecer os objetivos, comandos e demonstrações das regras de controle de acesso.
4. Acesse `Testes/` para consultar as evidências e os resultados registrados.

## Escopo e observações

Este é um projeto acadêmico de planejamento e simulação. Os resultados descritos devem corresponder ao que foi efetivamente configurado e testado no Packet Tracer. Recursos apenas planejados ou ainda não validados devem ser identificados como pendentes, sem serem apresentados como implementados.

Os valores de materiais e serviços presentes na documentação são estimativas para fins acadêmicos e podem variar conforme fornecedor, modelo, configuração, disponibilidade e condições comerciais.

## Autor

Projeto acadêmico desenvolvido como atividade de infraestrutura de TI.

