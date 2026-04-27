# LLM Cost Intelligence

An AI cost-aware intelligence SDK for predicting, tracking, and controlling LLM usage costs.

## Features
- Token-level cost estimation (tiktoken + fallback)
- Streaming cost tracking
- Budget-aware AI execution layer
- Redis usage logging
- Prometheus + OpenTelemetry telemetry
- LangChain integration hooks

## Example
```python
from llm_cost_intelligence.core import LLMCostIntelligence
from llm_cost_intelligence.ai_tool import AICostAwareTool

engine = LLMCostIntelligence("gpt-4o-mini")
tool = AICostAwareTool(engine, budget_per_request=0.01)

print(tool.run("Explain black holes"))
```
