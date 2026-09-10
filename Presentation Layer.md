- Operates at Layer 6 (Presentation Layer) of the OSI model
- Also called the Translation Layer or Syntax Layer
- Ensures proper data format, syntax, and semantics
- Provides encryption/decryption for security
- Applies compression to optimize bandwidth

## Functions of the Presentation Layer

Below are the functions of presentation layer:

- ****Data Translation****: Converts data from the application’s format into a standard network format (e.g., character encoding like ASCII ↔ Unicode) so different systems can understand each other.
- ****Data Compression****: Reduces the size of data before transmission using compression techniques, which saves bandwidth and improves transmission speed.
- ****Data Encryption/Decryption****: Encrypts data at the sender’s side to protect it from unauthorized access and decrypts it at the receiver’s side to restore readable information.
- ****Syntax and Semantics Management****: Ensures that data structure (syntax) and meaning (semantics) remain consistent between communicating systems, preventing misinterpretation.
- ****Transfer Syntax Negotiation****: Agrees on common data representation rules (format, encoding, compression method) before communication begins to ensure compatibility.
- ****Interoperability****: Enables communication between heterogeneous systems by handling differences in operating systems, data formats, and architectures.

## Presentation Layer Attacks

Since this layer deals with data formatting, compression and encryption, it is often targeted by attackers. Common attacks include:

- ****Man-in-the-Middle (MITM) Attacks:**** Interception of communication to steal sensitive data.
- ****SSL/TLS Downgrade Attacks:**** Forcing weaker encryption protocols.
- ****Certificate Spoofing:**** Using fake certificates to impersonate trusted entities.
- ****Code Injection:**** Exploiting vulnerabilities in data parsing or formatting.