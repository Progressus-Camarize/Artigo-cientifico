# 📄 Artigo Científico — Projeto Camarize

Artigo, apresentação e artefatos de projeto do **Camarize**, sistema de monitoramento IoT para carcinicultura desenvolvido pela equipe **Progressus** no curso de Desenvolvimento de Software Multiplataforma (DSM) da FATEC Registro.

![LaTeX](https://img.shields.io/badge/LaTeX-artigo-4F46E5?style=flat-square)
![Beamer](https://img.shields.io/badge/Beamer-slides-2563EB?style=flat-square)
![Licença](https://img.shields.io/badge/licença-MIT-7C3AED?style=flat-square)

## Documentos

| Documento | PDF | Fonte |
|---|---|---|
| **Artigo** — *Criação de Camarão em Cativeiro com Monitoramento IoT para Gastronomia* | [artigo.pdf](template-paper-f299-artigo/artigo.pdf) | [`template-paper-f299-artigo/`](template-paper-f299-artigo) |
| **Apresentação** (Beamer) | [apresentacao.pdf](template-beamer-f299-main/apresentacao.pdf) | [`template-beamer-f299-main/`](template-beamer-f299-main) |
| **Artefatos do projeto** | [artefatos.pdf](template-artefacts-f299-artefatos/artefatos.pdf) | [`template-artefacts-f299-artefatos/`](template-artefacts-f299-artefatos) |

## Sobre o artigo

O trabalho propõe um sistema de monitoramento e automação para cativeiros de camarão no Vale do Ribeira (SP): um ESP32 com sensores coleta temperatura, pH e amônia, envia os dados a uma API em nuvem e os disponibiliza em uma Aplicação Web Progressiva, com histórico em gráficos, alertas automáticos e controle de um dispensador de ração.

**Objetivos específicos**

1. Monitorar remotamente temperatura, pH e amônia, com alertas automáticos em caso de desvio.
2. Armazenar dados históricos e disponibilizar gráficos e relatórios.
3. Automatizar o fornecimento de ração, com horários e quantidades definidos pelo usuário.
4. Entregar uma aplicação web responsiva com acesso remoto em tempo real.

**Metodologia:** pesquisa aplicada, quantitativa e experimental. Validação em aquário com camarões e peixes, em seis testes, comparando o ESP32 com termômetro de aquário e kits químicos de referência.

**Principais resultados**

| Item | Resultado |
|---|---|
| Temperatura (DS18B20) | Precisão média de 98,27% (erro médio de 1,73%) |
| pH (Ph4502) | Precisão média de 95,98% (erro médio de 4,02%), com desvio de calibração praticamente constante |
| Amônia (MQ-135) | Sensor de gás inadequado para quantificação em meio aquático |
| Alerta ponta a ponta | Cerca de 2 minutos |
| Alimentador | Lógica de software correta; mecanismo físico instável |

Objetivos 1 e 3 foram atingidos parcialmente, e os objetivos 2 e 4 integralmente. A discussão completa, incluindo as limitações, está no [artigo](template-paper-f299-artigo/artigo.pdf).

## Artefatos de projeto

O documento de artefatos reúne, em um único PDF: Canvas, análise SWOT, UX/UI (guia de estilos e tipografia), estrutura do site, diagramas UML (casos de uso, classes, objetos, sequência, atividades, componentes, implantação e estados), modelagem de banco de dados (conceitual, lógico e físico) e DevOps (CI/CD, Docker Compose, arquitetura de deploy e monitoramento).

## Como compilar

Requer uma distribuição LaTeX ([TeX Live](https://www.tug.org/texlive/) ou [MiKTeX](https://miktex.org/)) com `latexmk` e BibTeX.

```bash
cd template-paper-f299-artigo
latexmk -pdf artigo.tex        # artigo

cd ../template-beamer-f299-main
latexmk -pdf apresentacao.tex  # slides

cd ../template-artefacts-f299-artefatos
latexmk -pdf artefatos.tex     # artefatos
```

## Repositórios relacionados

- [**APP-0.2-CAMARIZE-V2**](https://github.com/Progressus-Camarize/APP-0.2-CAMARIZE-V2): plataforma completa (API, painel web e firmware do ESP32)
- [**CAMARIZE-BY-PROGRESSUS**](https://github.com/Progressus-Camarize/CAMARIZE-BY-PROGRESSUS): site institucional do projeto

## Autores

Faculdade de Tecnologia do Estado de São Paulo — FATEC Registro

- Davi Mathais de Almeida
- Leandro Augusto de Souza Muniz
- Tiago de Lara Rodrigues