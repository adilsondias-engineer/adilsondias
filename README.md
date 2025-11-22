# Adilson Dias - Senior Integration Architect & FPGA Systems Engineer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/adilsondias/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black)](https://github.com/adilsondias-engineer)
[![Portfolio](https://img.shields.io/badge/Portfolio-FPGA%20Trading%20Systems-brightgreen)](https://github.com/adilsondias-engineer/fpga-trading-systems)

## 👋 About Me

Senior Integration Architect with **32 years of IT experience** (since 1993), combining deep technical expertise with active trading experience. Currently transitioning from MuleSoft enterprise integration to trading systems development.

**The Journey:**
- **1993:** Started as self-taught programmer at age 19 (Military Police, Ponte Nova, Brazil)
- **1999-2001:** Published 10 technical books (Delphi, C++ Builder, MySQL, Linux)
- **2008:** Active trading during financial crisis (DT Pro platform, built C# plugins)
- **2025:** Completed intensive FPGA trading systems portfolio (300+ hours, 14 projects)

**Current:** Senior Integration Architect @ Swinburne University (contract through May 2026)  
**Founded:** API-led Pty Ltd (2013) - Integration consulting business

## 🚀 Featured Project: FPGA Trading Systems

**Complete low-latency market data processing system** demonstrating production-grade architecture from FPGA hardware to multi-platform applications.

**Repository:** [github.com/adilsondias-engineer/fpga-trading-systems](https://github.com/adilsondias-engineer/fpga-trading-systems)

### Architecture Overview

```
FPGA Hardware (VHDL) → C++ Gateway → Multi-Protocol Distribution
         ↓                  ↓              ↓       ↓        ↓
   Ethernet PHY        UDP Listener    TCP:9999  MQTT   Kafka
   MII Interface       BBO Parser      Desktop  Mobile  Analytics
   ITCH Parser                          Java    .NET   (Reserved)
   Order Book                          ESP32    MAUI
```

### Key Achievements

**Hardware Layer (FPGA - Projects 6-8, 13):**
- ✅ UDP/IP Network Stack (< 2 μs wire-to-parsed, 100% reliability)
- ✅ NASDAQ ITCH 5.0 Parser (9 message types, symbol filtering)
- ✅ Hardware Order Book (120-170 ns order processing, 8 symbols)
- ✅ UDP BBO Transmitter (real-time distribution via MII TX)

**Application Layer (Projects 9-12, 14):**
- ✅ C++ Gateway UART (10.67 μs avg) → UDP (2.09 μs) = 5.1x faster
- ✅ RT Optimization (SCHED_FIFO + CPU isolation): 0.46 μs optimal
- ✅ Java Desktop Terminal (JavaFX with real-time charts)
- ✅ ESP32 IoT Display (Arduino, TFT, MQTT feed)
- ✅ Mobile App (.NET MAUI for Android/iOS/Windows)

### Performance Metrics (Hardware-Verified)

| Component | Latency | Validation |
|-----------|---------|------------|
| FPGA Pipeline | < 5 μs | Wire-to-BBO complete |
| Gateway (UART) | 10.67 μs | Baseline measurement |
| Gateway (UDP) | 2.09 μs | 5.1x improvement |
| Gateway (RT) | 0.46 μs | Multi-core isolation |

**Test Data:** Validated with authentic NASDAQ ITCH 5.0 data
- Source: 12302019.NASDAQ_ITCH50 (Dec 30, 2019 trading day)
- Dataset: 250M messages total, 50M in MySQL
- Test subset: 80,000 messages
- Symbols: AAPL, TSLA, SPY, QQQ, GOOGL, MSFT, AMZN, NVDA
- Result: 600+ msg/sec sustained, 100% accuracy

### Production Patterns Demonstrated

**FPGA Expertise:**
- Clock domain crossing (gray code FIFO synchronization)
- BRAM inference using Xilinx templates
- Multi-stage FSM pipelines for deterministic latency
- XDC timing constraints and closure
- Mixed-language integration (SystemVerilog/VHDL)

**Real-Time Optimization:**
- CPU isolation (GRUB: isolcpus, nohz_full, rcu_nocbs)
- SCHED_FIFO scheduling experiments
- Finding: CFS with 4 isolated cores optimal for ~400 msg/sec workload

**Systems Engineering:**
- Multi-threaded C++ (Boost.Asio async I/O)
- Binary protocol design (big-endian, fixed-point, UDP multicast)
- Multi-protocol distribution (TCP/MQTT/Kafka)
- Cross-platform development (Desktop/Mobile/IoT)

## 💻 Technical Background

### Languages (Actual Experience)
- **C++:** Since 1993 (32 years) - 200+ books collected, self-taught
- **Java:** Since 2000 (24 years) - J2EE, enterprise applications
- **Python:** 10+ years - automation, data processing, testing
- **VHDL:** 2025 (6 months intensive) - 300+ hours, 14 projects
- **C#:** DT Pro trading plugins (2008), .NET applications

### FPGA & Hardware
- **Platform:** Xilinx Arty A7-100T (Artix-7 FPGA)
- **Tools:** AMD Vivado Design Suite, ILA debugging
- **Protocols:** MII Ethernet, NASDAQ ITCH 5.0, UDP/IP
- **Skills:** CDC patterns, BRAM inference, timing closure

### Trading Background
- **Started:** 2002-2003 (Brazil market, phone-based)
- **Active Trading:** 2008-present (17 years)
- **Markets:** S&P 500, Nasdaq futures
- **Experience:** DT Pro platform, built C# trading plugins
- **2008 Crisis:** Real money trading during volatile markets
- **Domain Knowledge:** Order flow, market microstructure, spread dynamics

### Professional Certifications
- MuleSoft Platform Architect
- Salesforce Integration Architect  
- **Total:** 33 professional certifications

## 📚 Published Works

**Technical Author** - 10 books published 1999-2001 (Brazilian Portuguese)  
Editora Ciência Moderna

1. **Delphi para todas as versões** (1999) ISBN 85-7393-062-4
2. **Delphi Banco de Dados com SQL** (2000) ISBN 85-7393-073-X
3. **Dicas de Delphi** (2000) ISBN 85-7393-079-9
4. **WAP - A internet sem fios** (2000) ISBN 85-7393-093-4
5. **Desenvolvendo com Borland C++ Builder** (2000) ISBN 85-7393-095-0
6. **Desvendando WMLScript** (2000) ISBN 85-7393-101-9
7. **Imprimindo em Delphi** (2000) ISBN 85-7393-098-5
8. **Delphi & MySQL** (2000) ISBN 8573931094
9. **Banco de Dados com C++ Builder** (2001) ISBN 85-7393-120-5
10. **Kylix: A ferramenta Linux para programadores** (2001) ISBN 8573931426

## 🎓 Education & Background

**Post-Graduate Diploma**
- Java/J2EE Development - FIAP (São Paulo, Brazil)

**Bachelor of Sciences**
- Biology and Mathematics Education (1995-1998)
- Completed while working full-time at Military Police

**Self-Taught Journey (1993-present):**
- Started age 19 seeing green screen terminal at military police
- Traveled 330km from Ponte Nova to Belo Horizonte to buy programming books
- Self-taught: C/C++, Delphi, Clipper, dBase, Assembly, Linux
- Built first PC in 1994, learned on work computers before that
- 200+ C++ books collected over 32 years (pre-internet era)
- Deep Linux: Linux From Scratch, kernel compilation, Android porting

## 🏆 Career Timeline


**2025-2026: Senior Integration Architect** @ Swinburne University  
MuleSoft platform architecture, API-led connectivity

**2025-2025: Senior Integration Architect** @ Cbus Super  
MuleSoft platform architecture, API-led connectivity

**2015-2021: Senior Integration Architect** @ City of Melbourne (9 years)  
Enterprise integration, MuleSoft platform 

**2013-Present: Founder** @ API-led Pty Ltd  
Integration consulting business, IoT systems (26M+ data points, 99.8% uptime)

**2000-2015:** Various roles in systems integration  
Hexacta.com (B2B/B2C), Lear Corporation (Y2K mainframe migration), teaching positions

**1993-2000: Military Police & Programmer** @ PMMG (Minas Gerais, Brazil)  
Developed client-server applications while serving as soldier

## 🎯 Career Goals

Seeking **C++/Java trading development roles** leveraging:
- 32 years C++ experience (since 1993, self-taught)
- 17 years trading experience (2008-2025, real money)
- FPGA hardware acceleration expertise (300+ hours intensive development)
- Production systems experience (IoT: 26M+ data points)

## 💡 The Unique Combination

What differentiates me:

**Technical Depth:**
- 32 years professional software development
- Published technical author (10 books)
- Self-taught discipline (200+ C++ books, pre-internet era)
- Production systems (26M+ data points, 99.8% uptime)

**Trading Experience:**
- 17 years active trading (not paper trading)
- Built custom C# trading plugins (2008)
- Lived through 2008 financial crisis trading
- Understand market microstructure viscerally

**FPGA Skills:**
- 300+ hours intensive development (2025)
- 14 complete projects (hardware + software)
- Real NASDAQ data validation
- Production patterns: CDC, BRAM, timing closure

**The Story:**
Not "learning" trading systems - **returning to first principles**. Been interested in C++ + trading since 2002. Java dominated market (82% jobs vs 8% C++) so took rational path while preserving C++ knowledge. Now converging all domains: systems engineering + trading + FPGA.

## 🔗 Connect

- 💼 [LinkedIn](https://www.linkedin.com/in/adilsondias/)
- 🌐 [Website - dias.net.au](https://dias.net.au)
- 🌐 [Website - api-led.com.au](https://api-led.com.au)
- 💻 [GitHub](https://github.com/adilsondias-engineer)

## 📌 Featured Repository

### [fpga-trading-systems](https://github.com/adilsondias-engineer/fpga-trading-systems)
**300+ hours development, 14 complete projects**

- Sub-5μs FPGA wire-to-BBO latency
- 0.46μs C++ gateway (RT-optimized)
- Real NASDAQ ITCH 5.0 data processing
- Full-stack: Hardware → Gateway → Applications
- Complete documentation: architecture, benchmarks, lessons learned

---

## 💭 Philosophy

*"Why complicate if you can simplify"*

My approach to systems problems - whether enterprise integration, trading systems, or hardware acceleration.

---

**Currently Seeking:** C++/Java trading development roles  
**Location:** Melbourne, Victoria, Australia  
**Availability:** May 2026 (current contract ends) or 2 weeks notice  
**Can start discussions:** Immediately

**The 22-Year Story:** Started learning C++/trading in 2002. Took rational path through Java market (better opportunities). Now converging systems engineering + trading + FPGA. Not career change - **strategic return**.

![Profile Views](https://komarev.com/ghpvc/?username=adilsondias-engineer&color=brightgreen)
