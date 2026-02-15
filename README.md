# MultiLayerCryptoAuth

**Flask web application demonstrating multi-layer password encryption for authentication**

Educational project showing chained cryptography:  
**SHA-256** → **DES (ECB)** → **AES-256 (CBC)** → **RSA-2048 (raw deterministic)**

**Important**: This is **not secure for real-world use** (uses outdated DES, no salting, deterministic RSA). It's purely for learning layered crypto concepts.

### Features
- User registration with multi-stage password encryption
- Secure login verification (reverses the encryption chain)
- Session-based dashboard access
- Simple homepage showing user count
- Flash messages for user feedback

### Tech Stack
- Backend: Python + Flask
- Cryptography: pycryptodome (Crypto library)
- Frontend: Jinja2 templates + basic HTML
- Storage: Plain text file (users.txt) for demo purposes

### How to Run Locally
```bash
# Clone the repo
git clone https://github.com/LojainAhmad25/MultiLayerCryptoAuth.git
cd MultiLayerCryptoAuth

# Install dependencies
pip install flask pycryptodome

# Run the app
python app.py
