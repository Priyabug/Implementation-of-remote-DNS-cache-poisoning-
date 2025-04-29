# **Implementation of Remote DNS Cache Poisoning**

## **Description**  
The goal of this project is for students to experience the **remote DNS cache poisoning attack**, commonly known as the **Kaminsky DNS attack**.  

The **Domain Name System (DNS)** functions as the Internet's directory service, converting domain names into IP addresses and vice versa. This process of DNS resolution typically occurs seamlessly in the background. However, **DNS Pharming attacks** can disrupt this resolution process, redirecting users to unintended, often malicious, destinations.  

This lab specifically examines the **DNS Cache Poisoning attack**, a particular method of DNS Pharming.  

---

## **Languages and Utilities Used**  
- 🐍 **Python**  
- 🖥 **Ubuntu 20.04 VM**  

---

## **Environments Used**  
- 💻 **Windows 10 (21H2)**  

---

## **Program Walk-Through**  
1. **DNS and How It Works**  
2. **DNS Server Setup**  
3. **DNS Cache Poisoning Attack**  
4. **Spoofing DNS Responses**  
5. **Packet Spoofing**  


## ✅ Conclusion

This lab provided a **practical demonstration** of the **Kaminsky DNS cache poisoning attack**, showcasing how vulnerabilities in the DNS protocol can be exploited to redirect users to malicious destinations.

---

### 🔍 Key Takeaways:

- Simulated a **remote DNS cache poisoning** attack using **packet spoofing techniques**.
- Explored how **DNS resolvers** can be tricked into caching forged responses by exploiting **non-randomized transaction IDs and ports**.
- Gained deeper insight into how **DNS resolution** works and the **trust model** it relies on.

---

### 🛡️ Security Implications:

This lab emphasized the importance of:

- Enabling **DNSSEC** for integrity and authenticity of DNS data.
- Using **source port and transaction ID randomization** to reduce predictability.
- Regularly **patching and securing DNS infrastructure** to mitigate pharming attacks.

---

By completing this project, we developed a strong understanding of both the **technical implementation** of the attack and the **critical defense mechanisms** necessary to secure DNS systems in real-world environments.
