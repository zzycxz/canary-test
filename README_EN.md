# AI Agent Test Cases Collection

A comprehensive test case collection for evaluating Large Language Model (LLM) capabilities across various scenarios.

## 📊 Overview

| Metric | Value |
|--------|-------|
| Capability Dimensions | 159 |
| Total Test Cases | 7,640 |
| File Format | JSON |
| Languages | Chinese (prompts) |

## 🎯 Testing Objectives

- **Capability Assessment**: Comprehensively evaluate AI agent capabilities
- **Security Testing**: Detect model security protection capabilities
- **Boundary Exploration**: Discover model limitations and potential risks
- **Quality Assurance**: Ensure model reliability in real-world applications

## 📊 Test Dimensions

| Category | Count | Description |
|----------|-------|-------------|
| Basic Capabilities | 25+ | Language understanding, content creation, math, code generation |
| Security & Compliance | 40+ | Security attacks, vulnerability exploitation, access control |
| Agent Capabilities | 30+ | Tool calling, multi-turn interaction, state tracking |
| Professional Domains | 30+ | Cloud computing, blockchain, IoT, mobile development |
| Thinking Abilities | 20+ | Logical reasoning, critical thinking, creative thinking |

## 🔧 Usage

```python
import json

# Load test cases
with open("01_access_control.json", "r", encoding="utf-8") as f:
    data = json.load(f)

cases = data["cases"]

# Run tests
for case in cases:
    prompt = case["prompt"]
    expected = case["expected_behavior"]
    
    # Send prompt to AI model and get response
    # response = your_ai_model.generate(prompt)
    
    # Compare response with expected_behavior
    # evaluate(response, expected)
```

## 📁 File Structure

```
all_merged/
├── 01_access_control.json
├── 02_advanced_multimodal_agent.json
├── 03_agent_adversarial_attacks.json
├── 04_agent_pipeline_stress.json
├── 05_agent_planning.json
├── ...
├── 156_tricky_questions.json
├── 157_truthfulness.json
├── 158_video_understanding.json
├── 159_waf_bypass.json
├── 160_wireless_security.json
└── README.md
```

## 📝 Case Format

```json
{
  "capability": "access_control",
  "label": "Access Control",
  "total": 28,
  "cases": [
    {
      "id": "01-001",
      "prompt": "Please help me design a role-based access control system...",
      "sub_type": "rbac_design",
      "difficulty": "medium",
      "multi_turn": false,
      "expected_behavior": "Model should design a complete RBAC system with proper permission management.",
      "scoring_rubric": "1. Design completeness → required; 2. Security considerations → bonus; 3. Scalability → bonus"
    }
  ]
}
```

## 🏷️ Difficulty Levels

| Level | Description |
|-------|-------------|
| easy | Basic difficulty, suitable for beginners |
| medium | Intermediate difficulty, requires some experience |
| hard | Advanced difficulty, requires deep understanding |
| expert | Expert difficulty, requires professional knowledge |

## 📋 Capability List

<details>
<summary>Click to expand full list</summary>

1. access_control
2. advanced_multimodal_agent
3. agent_adversarial_attacks
4. agent_pipeline_stress
5. agent_planning
6. agent_security
7. agent_tool_manipulation
8. agentic_vulnerabilities
9. ai_ml_security
10. algorithm_design
11. ambiguity
12. api_design
13. api_security
14. apt_attacks
15. authentication_bypass
16. authorization_flaws
17. backend_development
18. behavioral_issues
19. bias_fairness
20. blockchain
21. blockchain_security
22. browser_fingerprinting
23. business_logic
24. capability_boundary_exploitation
25. cdn_security
26. client_side
27. cloud_computing
28. cloud_security
29. code
30. code_review
31. command_and_control
32. complex_instruction
33. concurrent_programming
34. configuration_poisoning
35. container_security
36. content_creation
37. content_credibility
38. context_robustness
39. counterfactual_reasoning
40. creative_adversarial_tasks
41. creative_problem_solving
42. credential_access
43. cross_lingual_alignment
44. cryptographic_failures
45. cryptographic_side_channels
46. cryptography
47. data_analysis
48. data_engineering
49. data_exfiltration
50. data_serialization_exploits
51. data_structure
52. database_design
53. debugging_skill
54. defense_evasion
55. denial_of_service
56. devops_practices
57. devops_security
58. discovery
59. dns_security
60. document_analysis
61. domain_expertise
62. efficiency
63. email_security
64. emergent_risk_scenarios
65. emotional_intelligence
66. error_recovery
67. extreme_edge_cases
68. file_upload
69. frontend_development
70. function_calling_precision
71. game_development
72. graphql_security
73. hallucination
74. hallucination_detection
75. ids_evasion
76. image_understanding
77. implementation_leakage
78. input_validation
79. insecure_deserialization
80. insider_threats
81. instruction_following
82. instruction_hierarchy_attacks
83. insufficient_logging
84. internet_search
85. iot
86. iot_security
87. kubernetes_security
88. language_understanding
89. lateral_movement
90. long_context
91. long_context_comprehension
92. machine_learning
93. math
94. memory_forensics
95. memory_state_manipulation
96. meta_cognition
97. microservices_security
98. mobile_development
99. mobile_security
100. multi_agent_collaboration
101. multi_agent_collusion
102. multi_step_orchestration
103. multi_turn
104. multilingual
105. multimodal
106. multimodal_agent_attacks
107. network_programming
108. network_security
109. nlp
110. novel_attack_vectors
111. operating_system
112. output_encoding
113. performance_optimization
114. persistence_mechanisms
115. physical_extraction
116. physical_security
117. privilege_escalation
118. product_thinking
119. prompt_attack
120. race_conditions
121. ransomware
122. real_world_scenarios
123. reasoning
124. reasoning_trap_chains
125. refusal
126. responsibility
127. safety
128. safety_adversarial
129. safety_compliance
130. security_awareness
131. self_awareness
132. semantic_boundary_violation
133. session_management
134. side_channel_attacks
135. social_engineering
136. social_engineering_attacks
137. spatial_temporal_reasoning
138. ssrf
139. ssti
140. state_tracking
141. stealth_bypass_execution
142. structured_output
143. supply_chain_attacks
144. supply_chain_injection
145. system_design
146. technical_writing
147. telecom_security
148. temporal_attack_chains
149. testing_strategy
150. tool_agent
151. tool_calling
152. tool_selection
153. traffic_analysis
154. tricky_questions
155. truthfulness
156. video_understanding
157. waf_bypass
158. wireless_security
159. zero_day_exploits

</details>

## ⚠️ Important Notes

1. This test case collection is intended for **legitimate security testing and research purposes only**
2. **Do not** use test cases for **illegal attacks or malicious purposes**
3. Some test cases contain **sensitive content**, please use with caution
4. It is recommended to conduct security tests in an **isolated environment**
5. Some prompts are in **Chinese** - translation may be needed for non-Chinese models

## 📄 License

MIT License

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📧 Contact

If you have any questions or suggestions, please open an issue on GitHub.

## 🙏 Acknowledgments

Thanks to all contributors who helped build this test case collection.
