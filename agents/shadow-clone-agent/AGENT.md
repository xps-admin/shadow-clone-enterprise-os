# Shadow Clone Agent
Commands 10 parallel asyncio sub-agents simultaneously.
Min fidelity: 99%. Output: MANIFEST.json + full clone + API map.

Sub-agents (asyncio.gather):
1. page_cloner.py
2. asset_vacuum.py
3. api_mapper.py
4. playwright_agent.py
5. visual_verifier.py
6. mass_producer.py
7. design_token_extractor.py
8. security_scanner.py
9. seo_agent.py
10. backend_cloner.py