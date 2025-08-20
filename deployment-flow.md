# Deployment Flow (Draft)

1. Upload model weights (e.g., Hugging Face → GCS).
2. Create model in Vertex AI Model Registry.
3. Deploy to endpoint (select machine type).
4. Send inference requests via REST API.
