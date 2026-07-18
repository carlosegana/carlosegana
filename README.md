<div align="center">

<img src="https://github.com/user-attachments/assets/c98c1d5c-c617-4cff-a2a6-c4c2dca635a9" alt="Carlos Egaña — AI Engineer" width="100%">

<br/><br/>

**AI Engineer** &nbsp;—&nbsp; LLM Systems · Agentic AI · Production Deployment

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=18&duration=3400&pause=1100&color=36BCF7&center=true&vCenter=true&width=860&lines=%24+whoami+--verbose;I+ship+LLM+systems+to+production%2C+not+just+notebooks;Agents+%C2%B7+MCP+%C2%B7+RAG+%C2%B7+Tool+use+%C2%B7+Evals" alt="Typing SVG">
</a>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0d1117?style=for-the-badge&logo=linkedin&logoColor=36BCF7)](https://www.linkedin.com/in/carlosegana)
&nbsp;
[![Email](https://img.shields.io/badge/Email-0d1117?style=for-the-badge&logo=gmail&logoColor=36BCF7)](mailto:carloseganac@gmail.com)
&nbsp;
[![Singapore](https://img.shields.io/badge/Singapore-0d1117?style=for-the-badge&logo=googlemaps&logoColor=36BCF7)](https://www.linkedin.com/in/carlosegana)

</div>

<br/>

## `> whoami`

```jsonc
// carlos@ai-engineer:~$ cat profile.jsonc
{
  "role":       "AI Engineer",
  "team":       "Data & AI — BDO Singapore",
  "domain":     "Enterprise GenAI: audit · tax · advisory · ESG",
  "focus":      ["Agentic systems", "MCP", "RAG", "LLM orchestration"],
  "language":   "Python-first",
  "background": "Information Systems & Control Management Engineering",
  "status":     "Shipping LLM systems to production"
}
```

**Agents, not chatbots.** I build agentic systems that plan, call tools, and execute multi-step workflows — function calling, MCP servers, and multi-agent orchestration over real enterprise data.

**Production over prototypes.** I own the full lifecycle: Python services → LLM integration → containerized deployment on AWS → monitoring, evals, and usage analytics.

**Enterprise constraints.** My systems survive real-world requirements: compliance, security reviews, cost control, and non-technical end users.

<br/>

## `> skills --matrix`

| `LLM_SYSTEMS` | `AGENTIC_AI` | `ENGINEERING` |
|:---|:---|:---|
| RAG pipelines & vector search | Multi-agent orchestration | Python services · FastAPI |
| Prompt engineering & evals | Tool use / function calling | Docker & containerization |
| Structured outputs & context mgmt | MCP — Model Context Protocol | AWS · ECR · App Runner |
| Claude API · OpenAI API | Agent evaluation & guardrails | Monitoring & usage analytics |

<br/>

## `> stack --list`

<div align="center">

**CORE ENGINEERING**

<img src="https://skillicons.dev/icons?i=python,fastapi,docker,aws,postgres,git&theme=dark" alt="Core Engineering"/>

**AI / LLM TOOLING**

[![Claude](https://img.shields.io/badge/Claude_API-0d1117?style=for-the-badge&logo=anthropic&logoColor=36BCF7)](#)
[![OpenAI](https://img.shields.io/badge/OpenAI_API-0d1117?style=for-the-badge&logo=openai&logoColor=36BCF7)](#)
[![MCP](https://img.shields.io/badge/MCP-0d1117?style=for-the-badge&logo=data:image/svg%2bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PGcgZmlsbD0iIzM2QkNGNyI+PGNpcmNsZSBjeD0iNSIgY3k9IjEyIiByPSIzIi8+PGNpcmNsZSBjeD0iMTkiIGN5PSI1IiByPSIzIi8+PGNpcmNsZSBjeD0iMTkiIGN5PSIxOSIgcj0iMyIvPjwvZz48ZyBzdHJva2U9IiMzNkJDRjciIHN0cm9rZS13aWR0aD0iMS44IiBmaWxsPSJub25lIj48cGF0aCBkPSJNNy42IDEwLjdMMTYuNCA2LjMiLz48cGF0aCBkPSJNNy42IDEzLjNMMTYuNCAxNy43Ii8+PC9nPjwvc3ZnPg==)](#)
[![LangChain](https://img.shields.io/badge/LangChain-0d1117?style=for-the-badge&logo=langchain&logoColor=36BCF7)](#)

<img src="https://skillicons.dev/icons?i=pytorch,tensorflow,sklearn,anaconda&theme=dark" alt="ML Frameworks"/>

**ANALYTICS & DATA**

[![Power BI](https://img.shields.io/badge/Power_BI_·_DAX-0d1117?style=for-the-badge&logo=data:image/svg%2bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0iIzM2QkNGNyIgZD0iTTMgMTNoNHY4SDN6TTEwIDhoNHYxM2gtNHpNMTcgM2g0djE4aC00eiIvPjwvc3ZnPg==)](#)
[![Tableau](https://img.shields.io/badge/Tableau-0d1117?style=for-the-badge&logo=tableau&logoColor=36BCF7)](#)
[![Alteryx](https://img.shields.io/badge/Alteryx-0d1117?style=for-the-badge&logo=alteryx&logoColor=36BCF7)](#)
[![SQL · R](https://img.shields.io/badge/SQL_·_R-0d1117?style=for-the-badge&logo=r&logoColor=36BCF7)](#)

</div>

<br/>

## `> agent --architecture`

```python
# The pattern behind every agentic system I ship
async def run_agent(task: Task) -> Result:
    context = retrieve(task, vector_store)          # RAG: ground the model in real data
    plan    = llm.plan(task, context)               # reasoning before acting

    for step in plan:
        tool   = registry.resolve(step)             # tool use via MCP servers
        result = await tool.execute(step.args)      # typed, validated I/O
        context.update(result)                      # feedback loop

    return evaluate(context.output)                 # evals + guardrails before delivery
```

<br/>

<!--
## `> featured --production`

PLANTILLA — reemplaza con tus 2-3 mejores repos públicos y descomenta la sección:

### ⚡ [Nombre del proyecto](link-al-repo)
`One-line:` qué hace y qué problema resuelve.
`Impact:` métrica o resultado concreto (usuarios, latencia, % mejora, adopción).
`Stack:` Python · FastAPI · Claude API · MCP · Docker · AWS
-->

## `> certs --verified`

| Certification | Provider | Year |
|:--------------|:---------|:-----|
| **OCI Generative AI Professional** | Oracle | `2025` |
| **OCI Data Science Professional** | Oracle | `2025` |
| **Certified in Cybersecurity (CC)** | ISC² | `2025` |
| **Digital Transformation Management** | Arizona State University | `2024` |
| **Data Science Practitioner · AI Practitioner** | IBM | `2024` |
| **Alteryx Designer Core** | Alteryx | `2024` |
| **Google Data Analytics Professional** | Google | `2023` |

<br/>

## `> principles --core`

```python
def build(problem):
    """How I approach every AI system."""
    solution = (
        understand(problem)          # business context before code
        .simplify()                  # smallest architecture that works
        .ship_early()                # production feedback > perfect prototypes
        .measure()                   # if it's not monitored, it's not done
    )
    return solution                  # reproducible · documented · owned end-to-end
```

<br/>

<div align="center">

## `> connect`

**Agentic AI · MCP · RAG Architecture · LLM Systems in Production**

*I discuss architecture, trade-offs, and what it actually takes to run GenAI in enterprise.*

[![LinkedIn](https://img.shields.io/badge/Connect_on_LinkedIn-0d1117?style=for-the-badge&logo=linkedin&logoColor=36BCF7)](https://www.linkedin.com/in/carlosegana)
&nbsp;
[![Email](https://img.shields.io/badge/carloseganac@gmail.com-0d1117?style=for-the-badge&logo=gmail&logoColor=36BCF7)](mailto:carloseganac@gmail.com)

<br/>

<img src="https://komarev.com/ghpvc/?username=carlosegana&color=36BCF7&style=flat-square&label=Profile+Views" alt="Profile Views">

</div>
