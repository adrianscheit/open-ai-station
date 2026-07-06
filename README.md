### 🛠️ The Desktop AI Station (Project: Open-AI-Local-Server Open-AI-Cassette)

This repository contains an early-stage concept and proposal for an open-source modular AI hardware accelerator ecosystem. The project is currently in the ideation phase.

The ultimate goal is to design an affordable, scalable, and fully local alternative for running AI models and autonomous AI agents directly on a desktop or inside an office.

### 🎯 Project Goals

*   **Affordable AI Compute:** Create a hardware alternative that allows small enterprises and private individuals to run advanced AI architectures locally, without relying on expensive enterprise hardware or cloud subscriptions.
*   **True Modular Expansion:** Define a standard for swappable hardware "cassettes" connected via a shared power and data bus. The objective is to allow near-limitless expansion of memory and computing power simply by sliding in additional modules.
*   **Local Privacy:** The system is intended to operate within a Local Area Network (LAN) via a network module. Local AI agents and desktop software can interact with the accelerator through a standard web API, keeping all data private and secure. The web interface will also be used for configuration, firmware updates, and a simple integrated chatbot feature.
*   **Healthy Market Competition:** By licensing the architecture under open-source terms, the goal is to allow any manufacturer to produce and sell these modules freely, forcing low consumer prices and high quality through open market competition.
*   **Right to repair** anyone that will own such station will be welcome and supported (passively) to maintain and fix it forever
*   **Focus on INT8** it seems like the sweat spot, at the begining, later it could support more formats dependent on the FPGA tests result

### 🗺️ Planned Development Phases

The project is structured into clear sequential stages to ensure long-term compatibility and architectural stability:

*   **Phase 1: Architecture & Logic Definition**  
    Formulating the shared data bus standards and establishing the basic compute core behavior.
*   **Phase 2: Basic Compiler Software & Open Model Standards**  
    Designing a specialized software compiler capable of taking open AI model standards (such as ONNX) and translating their computational graphs into optimized instructions for the hardware architecture.
*   **Phase 3: FPGA Functional Testing**  
    Implementing and testing accelerator logic in Verilog/SystemVerilog on accessible FPGA development boards to validate AI models running environment and the network part that would be just one for the station (that connectes 2.5Gb ethernet with the AI acceleration chips)
*   **Phase 4: Base Chip Design & Connector Standards**  
    Designing the foundational custom chip (ASIC), establishing the physical dimensions of the cassettes, and freezing the connector pinning standards to guarantee future backward and forward compatibility.
*   **Phase 5: Finishing the software goals**  
    So it can run smoothly in multiple enviroments, supporting viarity of AI models (ollama compatibility?? or even integration?? should be considered)
*   **Phase 6: Further iteration to make the solution more capable and usable**  
    This would return to Phase 2 or 3
    
### ⚖️ Proposed Licensing Strategy

To protect the open nature of the project while enabling commercial production:

*   **Hardware Concepts & Blueprints:** Intended to be licensed under **CERN-OHL-S v2** (Strongly Reciprocal).
*   **Software Toolchains & APIs:** Intended to be licensed under **GNU AGPL-3.0**.

* * *

*This is a living proposal. Feedback and architectural discussions from the open-source hardware community are highly welcome.*
