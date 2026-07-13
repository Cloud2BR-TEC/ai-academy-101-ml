# 06. Deploy and Score

After training and evaluating, the next 101 milestone is serving predictions.

## Minimum Deployment Path

1. Save and register the model artifact.
2. Create a scoring script (`score.py`).
3. Define runtime dependencies.
4. Deploy to an online endpoint.
5. Send test payloads and verify responses.

## Beginner Quality Checks

- Endpoint responds consistently.
- Input schema and output format are documented.
- Basic error logging is enabled.
- Cost awareness: stop or scale down unused resources.

## 101 Outcome

A working endpoint that can serve sample inference calls with reproducible setup steps.
