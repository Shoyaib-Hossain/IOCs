## Experiments / Methodology

### Conversational File-Upload Interaction

During the CTI analysis phase, a synthetic dataset was constructed in CSV format containing Indicators of Compromise (IOCs). These IOCs included IP addresses, file hashes, URLs, mutexes, registry keys, email addresses, user-agent strings, and JA3/JA4 fingerprints. The dataset combined IOCs previously extracted by the LLM from various threat intelligence reports with a larger set of synthetically generated fabricated IOCs across the same categories.

Each dataset was uploaded directly to the conversational LLM interface. A carefully designed prompt was then used to instruct the model to identify and match the compromised IOCs within the uploaded file.

Although programmatic access through official LLM APIs is also a possible option, this study does not aim to compare different methodological approaches. Instead, the Conversational File-Upload Interaction method was deliberately selected to evaluate the model’s native capability to process heterogeneous structured security events through direct file interaction.

This approach reflects common real-world cyber threat intelligence workflows, where analysts frequently receive or export heterogeneous structured security events in spreadsheet or CSV format from various sources, including SIEMs, threat intelligence platforms, and incident reports.

The experiment aims to demonstrate the extent to which current LLMs can support practical, low-barrier CTI workflows by assisting analysts in identifying relevant IOCs from structured security datasets without requiring additional programmatic integration.
