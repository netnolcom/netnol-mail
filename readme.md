<section align="center">
    <h2 align="center">
        <spam>Netnol Mail</spam>
        <br />
        <spam>
            <sup align="center"><sub><strong>Email secure beyond tomorrow</strong></sub></sup>
        </spam>
    </h2>
    <div>
        <h3>What is it?</h3>
        <p>Netnol Mail is a zero-knowledge, quantum-resistant email service built for an unbreakable inbox. Messages are
            encrypted so that only you can access them — no inspection, no interference, no breaches. Email designed to
            be truly private, intrusion-proof and leak-proof.</p>
    </div>
    <br />
    <div>
        <h3>Modules</h3>
        <p>The Netnol Mail architecture is decoupled into specialized services to ensure security, scalability, and
            cryptographic integrity:</p>
        <ul>
            <li><strong>Server:</strong> High-performance SMTP server responsible for receiving raw traffic and queueing
                data for processing.</li>
            <li><strong>Worker:</strong> Distributed task processor that manages the logic between the mail queue and
                the core infrastructure.</li>
            <li><strong>System:</strong> The central API core governing identity, ZKP verification, and public key
                management.</li>
            <li><strong>Client:</strong> Cross-platform interface where all client-side encryption and decryption occur,
                ensuring zero-trust.</li>
        </ul>
    </div>
    <br />
    <div>
        <h3>Technology</h3>
        <p>Netnol Mail implements a hybrid cryptographic stack designed to neutralize both current and future threats,
            ensuring that data is never persisted in a vulnerable state:</p>
        <ul>
            <li><strong>Kyber1024 (KEM):</strong> A lattice-based Key Encapsulation Mechanism providing post-quantum
                resistance, ensuring that secret exchanges remain immune to advanced quantum computing attacks.</li>
            <li><strong>AES-256-GCM:</strong> High-performance symmetric encryption with integrated authentication
                (GCM), used to secure message bodies and sensitive metadata.</li>
            <li><strong>Ephemeral Key Generation:</strong> The system generates random keys in runtime for each
                encryption session. These keys are encapsulated using the recipient's asymmetric public key; immediately
                after use, the clear-text version of the ephemeral key is purged from memory.</li>
            <li><strong>Read-Only Architecture:</strong> The key derivation and attachment process occurs in an isolated
                environment where the generated private key is never written to disk, serving only to seal the
                cryptographic package before permanent deletion.</li>
        </ul>
    </div>
    <br/>
    <div>
        <h3>Identity & Governance Framework</h3>
        <ul>
            <li>
                <h4>Sovereign Identity & Unified Access</h4>
                <p>
                    Authentication in Netnol Mail is anchored to the <strong>Netnol ID</strong>, the user’s immutable and sovereign identity root. Through a single login, the client locally decrypts access keys to provide a consolidated dashboard of all attached Organizations and inboxes. This aggregation occurs strictly on the client side; on the back-end, isolation is absolute. An Organization is mathematically incapable of detecting the existence of other organizations linked to the same ID. By utilizing <strong>Zero-Knowledge Proofs (ZKP)</strong>, the server validates identity without ever touching passwords or private keys, rendering individual accounts deliberately irrecoverable by any third party.
                </p>
            </li>
            <li>
                <h4>Organizational Architecture, MMK, and Plans</h4>
                <p>
                    All Netnol Mail instances operate on a unified <strong>Master Management Key (MMK)</strong> engine, with permission policies varying by plan. Upon registration, an <strong>Individual Organization</strong> is automatically pre-created. In this mode, the MMK operates in a restricted state, making it impossible to add any user other than the owner. While the owner can manage multiple inboxes, domains, and storage, all resources remain permanently tethered and limited to their specific ID. 
                </p>
                <p>
                    In <strong>Team and Enterprise</strong> plans, the MMK expands to allow administrators to attach inboxes to third-party IDs and manage external members. Since the technical foundation is identical, transitioning between plans (upgrade/downgrade) is a seamless reconfiguration of resource limits and MMK sharing permissions, requiring no data migration. Each Organization, including the personal one, maintains its own independent <strong>billing cycle</strong>, allowing a single user to manage personal and corporate contexts with total administrative autonomy and cost segregation.
                </p>
            </li>
        </ul>
    </div>
    <br/>
    <div>
        <h3>License</h3>
        <p>
            Netnol Mail is licensed under the <strong>AGPLv3</strong>. The primary motivation for this choice is to
            ensure that the project remains subject to <strong>public audit</strong> at all times. In a
            security-critical environment, transparency is not just a preference but a technical requirement; by keeping
            the source code open, we allow the global security community to verify our cryptographic implementations and
            Zero-Knowledge claims.
        </p>
    </div>
    <br />
    <br />
    <br />
    <div>
        <p align="center"><sup>Made with 💕 by Netnol</sup></p>
    </div>
</section>
