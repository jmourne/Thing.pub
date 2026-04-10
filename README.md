# Thing.pub
**Security-First Manuscript Management | Built-in Reader Feedback & Metrics**

## The Mission
**Thing.pub** is a grassroots, pro-bono initiative built to return control of intellectual property to its creators. Born from a personal need to secure manuscripts against a landscape of systemic piracy, unauthorized web-scraping, and invasive AI training, the platform provides authors with a hardened, secure home for their work. 

The mission is to provide professional-grade security without big-tech, corporate overhead and oversight. By utilizing a Trusted Backend model and strictly adhering to security standards like **NIST 800-53**, I am building an environment where authors can share their stories for review without the constant fear of IP theft.

### Core Objectives
* **Protect the Craft**: Utilize hardware-level device locking and **AES-256-GCM** encryption to ensure that a manuscript stays exactly where it was intended.
* **Forensic Accountability**: Through session-based watermarking and immutable audit trails, if a leak does happen, it is traceable and the party responsible can be held accountable.
* **Actionable Feedback**: Bridge the gap between security and insight by providing line-level critiques and automated reader metrics—without ever exposing raw text to selection or downloading.
* **Open-Source Integrity**: Favor open-source tools and simple, robust engineering to keep the platform sustainable, transparent, and accessible to authors regardless of their income.

### Core Security Features
* **Trusted Backend (Rust)**: A hardened security kernel that intercepts all requests, validates Supabase Auth JWTs, and manages cryptographic operations.
* **Device Locking**: Hardware fingerprinting restricts manuscript access to two unique devices, preventing account sharing.
* **Cryptographic Protection**: Manuscripts are encrypted at rest using **AES-256-GCM**. Decryption keys are managed via dedicated KMS logic and are never stored in the primary database.
* **Dynamic Watermarking**: Non-removable identifiers are tied to every reader account to ensure any potential leaks are forensically traceable.
* **Hardened Reader**: The frontend viewer disables text selection, right-clicking, downloads, and screen-capturing to mitigate piracy.
---
## Tech Stack
* **Rust**: Core security kernel and cryptographic operations.
* **Supabase**: Identity management, PostgreSQL database, and Row-Level Security (RLS).
* **TypeScript**: Client-side parsing and interactive reader dashboard.
* **SQLx**: Type-safe, direct database connections to prevent SQL injection at the compiler level.

## Reader Engagement & Feedback Intelligence
Data within **Thing.pub** is utilized strictly to help authors refine their craft and manage their distribution effectively. The focus is on providing insights into reader pacing and engagement so authors can identify where a story succeeds or where it may lose momentum.
* **Pacing & Engagement Insights**: Authors get data on where readers slow down or re-read sections. This helps identify high-impact scenes and areas that may require further structural refinement.
* **Custom Questions**: At the authors discretion, setup of specific questions or feedback requests can be set at the chapter level.
* **Reading Momentum**: Authors can view completion funnels to see the narrative drop-off rate. This ensures the manuscript maintains its pace through the final act and helps authors understand if their "hook" is working.
* **Read & Completion Tracking**: To ensure authors get the most our of feedback, the system tracks completion and read status per user. This allows creators to prioritize their review copies for readers who are actively engaged with the work.
* **Anonymized Aggregate Data**: Where specific individual metrics are not required for feedback, anonymized aggregate data shows general trends across the entire reader base without exposing individual reading habits.
* **Automated ARC Reviews**: To assist with launch day success, readers are prompted for a review immediately upon completion while the story is fresh. These reviews are stored and readers are provided with automated reminders to post their thoughts to public platforms on the book's official release day. _Future review platform integrations are being considered to automate this even more._ 

## Forensic Security
- **Device Locking:** Hardware fingerprinting restricts each access code to a maximum of 2 unique devices to reduce chances of account sharing and piracy.
- **Dynamic Watermarking:** A non-removable, unique cryptography that links the reader's unique access code to the version of the manuscript they view. This ensures total accountability. If a leak does occur, you know exactly who is responsible. 
- **Anti-Piracy Hardening:** Globally disabled text selection, right-click, screen cpature, and print-shielding.
- **No Downloads:** Because most security breaches happen on local devices, there is no download option for readers. All reading and feedback is contained within the secure app. 

## Project Philosophy
* **Grass-roots Development**: This platform is a pro-bono initiative built and maintained solely by **[Jules Mourne](https://threads.com/@jules.mourne)**. It is a personal mission of mine to return control of intellectual property to creators, providing authors with a hardened, secure home for their work.
* **Compliance-First**: We prove that professional-grade security does not require a corporate structure. The architecture is strictly mapped to **FedRAMP Moderate** and **NIST 800-53** standards, ensuring the integrity and confidentiality of manuscripts through a **Trusted Backend** and a **Micro-Enclave** security kernel.
* **Financial Transparency**: Platform access is free. To ensure long-term sustainability, I'll utilize a **Pay What You Want (PWYW)** model that allows community contributions to assist with infrastructure costs. A **public financial ledger** is maintained to provide real-time reporting on operating costs and funding allocation, ensuring full transparency with users.
---
## Contributing to Thing.pub
**Thing.pub** is currently in an active development phase, transitioning from an initial prototype to a scalable system. As a pro-bono project developed solely by **Jules Mourne**, community feedback is the primary driver for feature prioritization and security hardening.

I'm looking for early adopters and various experts to help stress-test the environment, refine the reader experience, and ultimately help shape the final product of what Thing.pub will be. Your input directly impacts the development.

### How to Get Involved
* **Provide Feedback**: Complete our [Early Adopter Survey](https://tally.so/r/ZjY0bv).
* **Stay Updated**: Follow the project's progress on [Substack](https://open.substack.com/pub/julesmourne) for regular updates on new features and milestones.
* **Review Documentation**: Explore our [System Security Plan](https://github.com/jmourne/Thing.pub/wiki/System-Security-Plan) and technical architecture to understand alignment with **NIST 800-53** standards.
* **Discord**: Link coming soon! (I am still setting the server up)
---
© 2026 Jules Mourne. Proprietary and Confidential.
