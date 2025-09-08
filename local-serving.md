# Local Serving (vLLM) — Draft

## Start server (conceptual)
```bash
pip install vllm
python -m vllm.entrypoints.openai.api_server --model meta-llama/Llama-3-8B-Instruct --port 8000

# Test request
curl http://localhost:8000/v1/completions \
  -H "Content-Type: application/json" \
  -d '{"model":"meta-llama/Llama-3-8B-Instruct","prompt":"Say hi","max_tokens":32}'
