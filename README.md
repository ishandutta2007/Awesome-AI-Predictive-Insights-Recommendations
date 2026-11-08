# Awesome-AI-Predictive-Insights-Recommendations

# Awesome-AI-Predictive-Insights-Recommendations

**Top AI Predictive Insights Recommendations (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Anomaly Detection, Revenue Forecasting, Unstructured Feedback Analytics & Self-Hosted Recommendation Engines*

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Predictive Insights & Recommendations**. These tools enable organizations to surface anomalies, forecast outcomes, extract themes from unstructured feedback, and recommend next-best actions—from fully managed platforms with proprietary ML models to open-source engines that give teams control over their models and data.



**Examples** include Dynatrace Davis AI, Datadog Watchdog, Salesforce Einstein Discovery, Gong Insights, Qualtrics XM Discover, Medallia, CallMiner Eureka, Freshworks Freddy AI Insights, Clari Copilot, and Balto (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted predictive analytics, recommendation engines, and open anomaly detection. **Critical note**: The open-source landscape splits by function—**Gorse** is the most complete open-source recommender system engine , **ParleML ml4** provides an AutoML engine with classification, forecasting, anomaly detection, and recommendation entry points , and **Security Shallots** offers lightweight AI-assisted anomaly triage for security telemetry . No open-source project matches Dynatrace's deterministic causal AI or Qualtrics's decade-trained NLP models, but for specific predictive capabilities, the building blocks exist.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **Dynatrace Davis AI**

  **Causal AI for root cause analysis** and anomaly detection. **Pricing**: **Per host and per feature module**; public list pricing is limited—formal quote required . **Estimated total cost**: **$80.5K–$203.2K first year** (base $126.5K); **$174.8K–$406.3K three-year total** . **Free tier**: Trial only. **Best for**: teams wanting deterministic root cause analysis rather than correlated alerts—**trade-off**: per-module pricing makes costs hard to forecast; learning curve is steep .



- **Datadog Watchdog**

  **Anomaly detection across metrics, APM, and logs**. **Pricing**: **Observability tiers start around $18/host/month** for the tier that includes Watchdog . **Free tier**: Limited trial. **Best for**: teams already on Datadog wanting anomaly detection without additional tooling—**trade-off**: **Watchdog detects anomalies but leaves root cause investigation to humans**; less automated than Davis AI .



- **Salesforce Einstein Discovery**

  **Automated insights and predictions** within Salesforce. **Pricing**: **~$25/user/month** for CRM Analytics Plus or Einstein Predictions licenses; **Sales Cloud Einstein $50/user/month** (billed annually) . **Free tier**: Developer Edition available. **Best for**: Salesforce customers wanting predictive models on CRM data—**trade-off**: requires minimum 400 rows of outcome data for model creation; maximum 20M rows and 50 columns .



- **Gong Insights**

  **Revenue intelligence analytics module** within Gong. **Pricing**: **Add-on to core Gong subscription**—estimated **$15K–$40K/year** depending on module . **Free tier**: None. **Best for**: Gong customers wanting deeper analytics and benchmarking on conversation data—**trade-off**: module costs stack significantly; core Gong subscription required first .



- **Qualtrics XM Discover**

  **Unstructured text and speech analytics** (originally Clarabridge). **Pricing**: **Quote-only**; requires existing XM Discover subscription for Azure SSO integration . **Free tier**: None. **Best for**: organizations processing large volumes of contact center transcripts, open-text surveys, and social feedback—**trade-off**: **most mature AI layer in the Qualtrics stack**; multi-language support mature for major European languages but developing for others .



- **Medallia**

  **Experience management** with speech analytics. **Pricing**: **No publicly posted prices**—pricing page describes Experience Data Record (EDR) pricing with unlimited users and directs buyers to "Talk to Sales" . **Free tier**: None. **Best for**: enterprises with dedicated CX programs wanting feedback analytics—**trade-off**: annual-tier pricing only; no public rates .



- **CallMiner Eureka**

  **Speech and text analytics** for contact centers. **Pricing**: **Pricing available upon request**; no plan information publicly available . **Free tier**: None. **Best for**: contact centers needing 100% call inspection and compliance monitoring—**trade-off**: quote-only; enterprise sales process .



- **Freshworks Freddy AI Insights**

  **AI insights within Freshdesk/Freshservice**. **Pricing**: **Included in Enterprise tier only**; no separate add-on price. **Cheapest published plan carrying Freddy AI Insights**: **Freshdesk Omni Enterprise $119/agent/month billed annually** . **Free tier**: No—Enterprise only. **Best for**: Freshworks Enterprise customers wanting root cause analysis and customized insights—**trade-off**: requires Enterprise tier; no standalone purchase .



- **Clari Copilot**

  **Conversation intelligence** within Clari revenue platform. **Pricing**: **Starting price ~$500/user/year** per SourceForge listing; Software Advice lists $80/month or $1,080/year (product comparison may differ) . **Free tier**: None. **Best for**: Clari customers wanting call insights alongside forecasting—**trade-off**: pricing data conflicts across sources; verify directly .



- **Balto**

  **Real-time guidance** for contact center agents. **Pricing**: **Custom pricing only**—"what you pay depends on your team size and how you work"; phone system integration required . **Free tier**: None. **Best for**: contact centers wanting live agent coaching—**trade-off**: custom pricing only; implementation complexity .



## Open-Source GitHub Projects



- **Gorse**

  **Open-source recommender system engine** (Apache 2.0) — **the most complete open-source recommendation engine**, designed to be quickly introduced into online services . **Features**: **Multi-source recommendation**—popular, latest, user-based, item-based, and collaborative filtering, ranked by click-through rate prediction; **AutoML**—automatically chooses the best recommendation model and strategy via background model searching; **distributed recommendation**—single-node training, distributed prediction, horizontal scaling; **RESTful API** for data CRUD and recommendation requests; **dashboard** for data import/export, monitoring, and cluster status . **Tech stack**: Go. **Deploy**: Self-hosted (Docker Compose, manual); stores data in MySQL, MongoDB, PostgreSQL, or ClickHouse with Redis caching . **Trade-off**: **Recommendation-focused**—no built-in anomaly detection or forecasting; requires data ingestion pipeline. **Best for**: developers wanting to add personalized recommendations to their application—the most mature open-source recommender engine available.



- **ParleML ml4**

  **AutoML training engine driven by AI agents** (PyPI, free including commercial use) — **the most comprehensive open-source predictive analytics engine** found in this research, with dedicated entry points for every common ML task . **Features**: **One entry point per task**—classification/regression (`AutoSupervised`), time-series forecasting (`Forecaster`), **anomaly detection** (`AnomalyDetector`), clustering (`ClusteringDetector`), **recommendation** (`Recommender`), learning-to-rank (`LTRRanker`), association rules (`AssociationMiner`); **leakage-safe feature engineering**—domain parsers for IP, geography, emails, names, addresses, phone, card, IBAN, dates; **post-fit layer**—calibration, decision-threshold tuning, prediction intervals, baseline checks; **regulated models**—glass-box models (GLM, scorecard, RuleFit, EBM) with monotonic constraints for compliance; **forecasting** with four backends including Chronos foundation model; **hyperparameter search** with Optuna, AutoGluon, or good defaults . **Tech stack**: Python 3.11–3.13 (Windows/Linux x86-64; macOS via Docker) . **Deploy**: `pip install parleml-ml4`; Python API . **Trade-off**: **Library, not a platform**—no UI, no scheduling, no data connectors; requires ML engineering. **Best for**: developers and data scientists wanting a single engine for anomaly detection, forecasting, recommendation, and classification—especially those needing regulated glass-box models for compliance.



- **Security Shallots**

  **Lightweight, self-hosted SIEM with AI-assisted anomaly triage** (PyPI) — **the easiest entry point to AI-assisted anomaly detection**, running on anything from a Raspberry Pi to a server . **Features**: **Ingests** Suricata, Syslog, pfSense, Wazuh, CrowdSec, Pi-hole, Argus agents, and web logs; **normalizes, deduplicates, auto-classifies severity**; **correlates patterns** (port scans, brute force, lateral movement); **groups into incidents** with runbooks; **AI triage via API** (OpenAI/Anthropic) or local Ollama—no GPU needed; **hardware auto-detection** adjusts profile based on RAM/CPU . **Profiles**: Lite (<2 GB, Suricata+syslog); Full (8+ GB, baselines, graph, ML) . **Tech stack**: Python, SQLite . **Deploy**: `pip install .`; `shallot run`; systemd service . **Trade-off**: **Security-focused anomaly detection**—not general business insights or recommendations; SQLite limits retention at high volume . **Best for**: homelabs, small businesses, and security teams wanting AI-assisted anomaly triage without Elastic or Splunk infrastructure—especially those starting on minimal hardware.



### Additional Strong Open-Source Options



- **No mature open-source equivalent to Dynatrace Davis AI or Qualtrics XM Discover exists.** Those platforms bundle years of proprietary model training and enterprise integrations that open-source projects cannot replicate. **Gorse** and **ParleML ml4** provide specific capabilities (recommendation, anomaly detection) but not a unified insights platform.



**Frameworks for building custom systems**: Combine **ParleML ml4** for anomaly detection and forecasting with **Gorse** for recommendations and **Security Shallots** for security-focused anomaly triage—creating a layered open-source predictive analytics stack. **None of these match Dynatrace's causal AI or Qualtrics's NLP depth**, but for specific predictive tasks, the options are production-capable.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- AI predictive insights platforms handling business and customer data must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls.

- **The "causal AI" vs. "anomaly detection" vs. "automated insights" vs. "unstructured text analytics" vs. "recommendation engine" distinction is critical.** **Dynatrace Davis AI** provides **causal AI**—deterministic root cause analysis across the tech stack . **Datadog Watchdog** provides **anomaly detection**—it surfaces anomalies but leaves root cause to humans . **Salesforce Einstein Discovery** provides **automated insights**—it examines variable combinations to find predictive patterns . **Qualtrics XM Discover** and **CallMiner Eureka** provide **unstructured text/speech analytics**—theme extraction, sentiment, and intent from conversations . **Gorse** and **ParleML ml4** are **open-source engines**—recommendation and AutoML respectively . **Choose based on whether you need root cause, anomaly surfacing, predictive patterns, text analytics, or recommendations.**

- **Dynatrace's cost is substantial**—estimated **$80.5K–$203.2K first year**, **$174.8K–$406.3K three-year** . **Model total cost including implementation, integration, and staff time before committing** .

- **Datadog Watchdog is an overlay, not a replacement for Davis AI**—it detects anomalies but leaves root cause investigation to humans; less automated than Dynatrace . **The trade-off**: cheaper entry (~$18/host/month) but more analyst time.

- **Gong Insights costs $15K–$40K/year as an add-on**—stacked on top of core Gong subscription . **Model total cost before committing; module costs can rival the base platform** .

- **Freshworks Freddy AI Insights requires Enterprise tier**—cheapest entry is **Freshdesk Omni Enterprise at $119/agent/month annual** . **No standalone purchase available** .

- **Qualtrics XM Discover is the most mature AI layer in the Qualtrics stack**—built on Clarabridge's decade of NLP, production-quality for English, mature for major European languages . **The trade-off**: quote-only; multi-language support developing for others .

- **ParleML ml4 is the most comprehensive open-source predictive engine**—one API for classification, forecasting, anomaly detection, recommendation, clustering, and ranking, with regulated glass-box models . **The trade-off**: library, not platform; requires ML engineering. **For teams wanting a single engine for multiple predictive tasks, it is the strongest starting point.**

- **Gorse is the most mature open-source recommender engine**—AutoML, distributed prediction, REST API, and dashboard . **The trade-off**: recommendation only; no anomaly detection or forecasting.

- Self-hosted open-source solutions require proper infrastructure (Go for Gorse, Python for ParleML and Shallots), security hardening, and ongoing maintenance. **Predictive insights platforms process business telemetry and customer data**—ensure your deployment meets your organization's privacy and compliance requirements before processing production data.



---



**Made for data scientists, analytics teams, and organizations building transparent predictive insights solutions.**

Let's make AI Predictive Insights & Recommendations more open, data-driven, and action-oriented.
