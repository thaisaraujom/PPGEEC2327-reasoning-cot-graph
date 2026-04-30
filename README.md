# Trabalho 02 - Parte 02

## Cadeias de Raciocínio em Reasoning Models

**Tema:** Reasoning AI, LLM/SLM e Knowledge Graph  
**Estudo de caso:** Cadeias de raciocínio em modelos de linguagem: explicação fiel ou racionalização convincente?

## Membros do grupo

- Alice Freire
- Erick Justino
- Maria Luz
- Thaís Medeiros

## Descrição do projeto

Este repositório contém os artefatos do estudo de caso desenvolvido para a disciplina. O objetivo foi analisar como a literatura científica discute a relação entre cadeias de raciocínio (Chain-of-Thought), explicabilidade e fidelidade em modelos de linguagem e reasoning models.

O trabalho utilizou o Graphify como ferramenta de apoio para transformar um conjunto de artigos científicos em um grafo de conhecimento. A partir do grafo, foram analisados os principais nós, as relações, as comunidades temáticas e as evidências sobre a diferença entre efetividade da CoT e fidelidade da CoT.

As mesmas perguntas de análise também foram exploradas no NotebookLM, como apoio comparativo qualitativo. O objetivo desse uso adicional foi verificar se a leitura textual dos artigos reforçava ou tensionava os padrões observados no grafo gerado pelo Graphify.

## Pergunta que guiou a busca dos artigos

Como a literatura científica revisada por pares discute a relação entre cadeias de raciocínio (CoT), explicabilidade e fidelidade em modelos de linguagem/reasoning models?

## Perguntas que guiaram a exploração do grafo

1. Como a literatura conecta cadeias de raciocínio, explicabilidade e fidelidade?
2. As cadeias de raciocínio aparecem mais como explicações fiéis ou como racionalizações plausíveis?
3. Como a literatura diferencia efetividade da CoT e fidelidade da CoT?

## Corpus analisado

O corpus foi composto por 8 artigos científicos sobre Chain-of-Thought, explicabilidade, fidelidade, reasoning models e avaliação de raciocínio.

Os PDFs estão em:

- `data/papers/`

Os textos extraídos dos PDFs estão em:

- `data/corpus-text/`

## Ferramentas utilizadas

- **Graphify:** ferramenta principal utilizada para gerar o grafo de conhecimento, identificar comunidades, produzir o relatório e exportar as visualizações.
- **NotebookLM:** ferramenta utilizada como apoio comparativo qualitativo, a partir das mesmas perguntas aplicadas ao corpus, para contrastar respostas textuais com os padrões estruturados observados no grafo.

Observação: recursos como **NetworkX** e **Leiden community detection** fazem parte do pipeline interno do Graphify. Eles não foram utilizados como ferramentas separadas, mas aparecem no processo porque o Graphify os utiliza para estruturar o grafo e identificar comunidades.

## Resultados principais

O Graphify retornou:

- 135 nós
- 189 arestas
- 8 comunidades
- 85% de relações extraídas diretamente dos textos
- 15% de relações inferidas
- 1% de relações ambíguas

Principais nós identificados:

- `Error Recovery`
- `NLE Faithfulness`
- `Output-level Self-consistency`
- `Active Guidance`
- `Confidence Trajectories`
- `Unfaithful Recovery`
- `Explanation Faithfulness`
- `Reasoning Faithfulness`
- `Generative CoT Evaluation`
- `CoT Effectiveness`

## Principais insights

- CoT melhora a compreensibilidade, mas não garante fidelidade.
- Efetividade da CoT e fidelidade da CoT são dimensões diferentes da análise.
- A literatura trata cadeias de raciocínio como explicações que precisam ser verificadas.
- O grafo evidenciou relações entre fidelidade, racionalização, avaliação, grounding em grafos de conhecimento e recuperação de erros.
- O Graphify ajudou a organizar a literatura em comunidades temáticas e a revelar padrões de análise.

## Apoio comparativo com NotebookLM

Além da exploração com Graphify, as três perguntas principais também foram submetidas ao NotebookLM. As respostas obtidas reforçaram os principais achados observados no grafo:

1. **CoT, explicabilidade e fidelidade:** o NotebookLM destacou a tensão entre explicações plausíveis e explicações fiéis. A CoT aumenta a aparência de transparência, mas a literatura problematiza se essa explicação textual representa de fato o processo interno do modelo.
2. **Explicação fiel ou racionalização plausível:** as respostas apontaram que a literatura recente tende a tratar muitas cadeias de raciocínio como racionalizações plausíveis ou explicações pós-hoc, especialmente quando há omissão de vieses, recuperação infiel de erros ou trajetórias de confiança que indicam decisão prévia.
3. **Efetividade versus fidelidade:** o NotebookLM também reforçou a separação entre desempenho e fidelidade. Uma CoT pode ajudar o modelo a chegar a uma resposta correta ou mais organizada, mas isso não comprova que a explicação textual seja fiel ao processo que gerou a resposta.

Essa comparação foi útil porque o Graphify evidenciou os padrões de forma estruturada, por meio de nós, arestas e comunidades, enquanto o NotebookLM produziu uma síntese textual mais direta dos mesmos debates. Assim, o NotebookLM foi usado como apoio interpretativo, e não como substituto da análise estruturada do grafo.

As respostas completas registradas a partir do NotebookLM estão em:

- `docs/notebooklm_respostas.md`

## Limitações

- O corpus foi menor e focado, o que favorece profundidade, mas reduz abrangência.
- O grafo simplifica nuances teóricas presentes nos artigos.
- Relações inferidas e ambíguas precisam de validação crítica.
- O Graphify foi utilizado como apoio à análise, não como fonte de verdade absoluta.
- A comparação com NotebookLM foi qualitativa e exploratória, sem uma avaliação sistemática entre ferramentas.

## Estrutura do repositório

```text
.
├── README.md
├── slides/
│   └── PPGEEC2327_T2.pdf
├── data/
│   ├── papers/
│   └── corpus-text/
├── docs/
│   ├── notebooklm_respostas.md
│   └── roteiro_apresentacao.docx
├── results/
│   └── graphify/
│       ├── GRAPH_REPORT.md
│       ├── graph.html
│       ├── graph.json
│       ├── graph.svg
│       └── memory/
└── references/
    └── REFERENCES.md
```

## Artefatos principais

- Slides: `slides/PPGEEC2327_T2.pdf`
- Grafo interativo: `results/graphify/graph.html`
- Grafo em SVG: `results/graphify/graph.svg`
- Grafo estruturado: `results/graphify/graph.json`
- Relatório do Graphify: `results/graphify/GRAPH_REPORT.md`
- Respostas do NotebookLM: `docs/notebooklm_respostas.md`
- Roteiro da apresentação: `docs/roteiro_apresentacao.docx`
- Referências: `references/REFERENCES.md`
