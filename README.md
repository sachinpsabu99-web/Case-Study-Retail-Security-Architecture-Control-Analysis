CASE STUDY: RETAIL SECURITY ARCHITECTURE & CONTROL ANALYSIS

EXECUTIVE SUMMARY

This report provides a comprehensive security audit of a modern retail financial environment. As a Customer Service Manager with a background in Cybersecurity (Postgraduate Diploma, Dublin Business School) and Computer Applications (MCA), I conducted this analysis to evaluate how theoretical security principles such as Defense in Depth and Least Privilege are applied in a high-stakes live operational setting.



1. PROJECT OVERVIEW
   
   Location: Major UK/Ireland Retail Financial Branch.
   
   Objective: To identify and categorize the technical, administrative and physical security controls used to protect sensitive financial transactions and customer data.
   
   Tools Identified: CrowdStrike Falcon (EDR), StarMicronics Configuration Utilities and Windows Group Policy Objects (GPOs).

2. DEFENSE IN DEPTH: LAYERED SECURITY ANALYSIS

    Layer 1: Administrative Controls (People & Policy)

     The "Human Layer" is secured through strict corporate policies and incentivized training

      - Security Awareness: Regular security awareness classes are mandatory for all staff members.
  
      - Compliance Incentives: Staff are ineligible for bonuses if they fail to complete mandatory security training.
  
      - Managed Access: Accounts are automatically blocked after multiple failed login attempts requiring direct contact with the IT department for restoration.

    Layer 2: Physical Security

     Physical monitoring ensures accountability and protects hardware assets

      - Dual-Zone Surveillance: A dedicated CCTV system monitors employees while a separate system monitors customers and the general shop area.
  
      - Hardware Lockdown: Access to thermal printer configuration and USB serial number setting tools is restricted to specific utility folders.

    Layer 3: Identity & Access Management (IAM)

     The system enforces strict authentication boundaries to prevent unauthorized entry

      - Credential Separation: Employees use unique logins for the till and separate credentials for the clock-in/out system.
  
      - Dynamic Rotation: Till passwords expire every 30 days to prevent tracking while time-management credentials expire every two months.
  
      - Service Authentication: Secondary username and password prompts are required for accessing corporate email or material ordering applications.
  
    Layer 4: Endpoint Security

     The workstation environment is heavily restricted to minimize the internal attack surface

      - Endpoint Detection and Response (EDR) Protection: The systems are equipped with CrowdStrike Falcon for real-time malware scanning and threat detection.
  
      - System Restrictions: Users are blocked from opening system settings or accessing system properties due to administrative restrictions.
  
      - Data Loss Prevention (DLP): "Copy and Paste" functions are disabled system-wide to prevent unauthorized data movement.
  
      - Information Obfuscation: Disk partitions are hidden and standard folders (Music, Pictures, Videos) are kept empty to prevent local data storage.

    Layer 5: Network & Web Security

     Egress filtering and browser lockdowns prevent exposure to external threats so that sensitive data does not leave the network.

     - Content Filtering: Entertainment and social media platforms (YouTube, Facebook, Instagram) are blocked at the network level.
  
     - Forced Intranet: The search engine is locked to the corporate home page for both initial launch and every new tab opened.
  
     - Secure Browsing Protocol: Employees must use incognito tabs for any necessary general internet searches to minimize session tracking.
  
     - Wi-Fi Management: The shop Wi-Fi is configured to automatically disconnect after a set period of time.
  
     - Encryption Observations: Identified a "Privacy Error" on internal career domains despite the presence of HTTPS indicating a potential area for certificate management improvement.
  
 3. PROFESSIONAL TAKEAWAYS

    This audit demonstrates a robust "Zero Trust" architecture in a retail setting where

       - Least Privilege is enforced by stripping user rights to the operating system.

       - Continuous Monitoring is achieved through integrated CCTV and enterprise EDR tools.

      -  Risk Mitigation is managed by isolating personal internet use from critical corporate tasks.

  
