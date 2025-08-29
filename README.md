# Blockchain-Based Supply Chain Transparency for Agricultural Produce

## Description
A decentralized platform to track agricultural produce from farm to consumer, offering full transparency in pricing, quality, and origin. This solution empowers farmers, distributors, retailers, and consumers to verify produce events, reduce exploitation, and prevent fraud throughout the supply chain.

---

## Table of Contents
- Features
- Architecture
- Workflow
- Usage
- Technical Details
- Testing
- Roadmap
- License
- References

---

## Features
- Immutable product records (origin, harvest, processing, transport, sale)
- Transparent smart-contract powered fair pricing
- QR code integration for instant product traceability
- User-friendly web/mobile dashboards for all stakeholders
- Deployable on low-cost hardware or cloud infrastructure

---

## Architecture
- **Application Layer:** Stakeholder interfaces (web/mobile)
- **Blockchain Layer:** Ethereum smart contracts, identity management
- **Infrastructure Layer:** Raspberry Pi/local servers or AWS/Azure cloud (Isme hum jo website hoga user level me usko host karega ,using apache(if raspberry pi) and all as a server)
- **IoT/QR Layer:** Sensor data (quality/location) and secure QR code generator

---

## Workflow
- We will assign a ERC721(non fungible aur contains metadata of the crop) token to every packet of the crop, which will be used to update and track the packet or the status of the plant
- And the metadata of the token would be used as the metadata of the qr code which is mapped to the crop
  
1. **Farmer:** Registers produce, uploads crop data, certifications
2. **Distributor:** Logs quality checks, shipping, and handovers
3. **Retailer:** Updates shelf life, prints QR codes
4. **Consumer:** Scans QR to view full lifecycle and feedback
5. **Smart Contract:** Automates payments, validates events

---


## Usage

- **Farmers:** Register and update produce information
- **Distributors:** Add transport/inspection details and Generate the QR code with its metadat : Factories
- **Retailers:** Manage produced QR codes and the supply chain to the consumers : Shop and Markets
- **Consumers:** Scan QR for verification
- **Admins:** Audit, monitor, and report through dashboards
- **Helpline and complains :** Any party involved in the process from farmer to the consumers can complain using the tracking token

---

## Technical Details

- Smart contracts automate record creation and payments
- Each transaction is cryptographically signed and timestamped and will be available in the public ledger which can be accessed using the etherscan 
- QR codes function as digital fingerprints of produce batches
- System scalable for millions of transactions via cloud deployment

---

## Testing

- Unit tests for each smart contract and ledger event (Foundry)
- End-to-end simulated supply chains with real data
- Stakeholder usability workshops and iterative UI/UX improvements

---

## Roadmap

- [ ] Integrate IoT sensors for live quality monitoring
- [ ] Implement direct farming cost transparency to avoid overpriced packaging of the crops by the distributors
- [ ] Expand to more crops and locations

---


## References

- Authenticity in Food Supply Chain Using Blockchain[https://github.com/lakshya-20/supply-chain]
- Blockchain technology for agricultural supply chains[https://pmc.ncbi.nlm.nih.gov/articles/PMC8908783/]
- Blockchain Secure QR Code Generator For Farming[https://farmonaut.com/precision-farming/blockchain-secure-qr-code-revolutionize-farming-now]
- Blockchain-based solution for Indian agricultural supply chains[https://sist.sathyabama.ac.in/sist_naac/aqar_2022_2023/documents/1.3.4/b.e-cse-batchno-84.pdf]

---

# Technology Prerequisites for Blockchain-Based Agricultural Supply Chain Project

| Technology Name                     | Use in Project                                                                                                                          |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| **Ethereum**   | Core blockchain ledger to securely record produce lifecycle events and enable smart contracts                                           |
| **Smart Contracts (Solidity)** | Automate verification, payments, and milestone tracking through encoded supply chain rules                                              |
| **Node.js, Python**                 | Backend programming for APIs, transaction processing, and web/mobile app logic                                                          |
| **Web Frameworks (React, Angular, Django)** | Develop user-friendly dashboards and portals for farmers, distributors, retailers, and consumers                                        |
| **QR Code Generator/Reader (python-qrcode, ZXing, Google Vision)** | Generate and scan QR codes linked to blockchain entries for instant produce traceability                                               |
| **IoT Sensors (DHT22, GPS, Soil Moisture Sensors)** | Capture real-time environmental and location data for crops and transportation                                                          |
| **Database (MongoDB, MySQL, PostgreSQL)** | Store off-chain user data, metadata, and analytics complementing the blockchain ledger                                                     |
| **Cloud Services (AWS, Azure, GCP)** | Host blockchain nodes, databases, and APIs to ensure scalable and reliable deployment                                                     |
| **Mobile Devices (Smartphones, Tablets)** | End-user access tools to scan QR codes, submit data, and interact with traceability dashboards                                           |
| **Satellite Imaging APIs**          | Integrate objective land and crop data to enhance produce verification                                                                    |
| **Security Libraries (OpenSSL, JWT)** | Ensure secure data transactions, identity verification, and encrypted communications                                                       |

---

# Team Members and Its Role : 
- James Lego(Blockchain Ops) : Ethereum & Smart Contracts, Testing(forge) , Devops, scripts(cast) and Foundry, Local chain Deployment(anvil)
- Pankaj Kumar(Backend Ops) : Javascript(Node.js,web3.js,ether.js) integration of metamask wallet with the smart contracts
- Aryan(Frontend and Database) : React & web Frameworks & Database operations
- Nishchay(Hardware and AWS) : IOT sensors and deployment to the cloud
- komal (APIs) : satellite Imaging APIs and Generation of QR codes 

---

# Note
@members The roles are interchangable and not finalized

@dev It is recommended to be familiar with all the technology mentioned above


