# Date - 27 June 2024
# SECURING WIRELESS NETWORKS

# Day 11: Securing Wireless Networks
Wireless network security was the topic of today’s session, and it’s more complex than I initially thought. We started by discussing how wireless networks operate and the security risks associated with them. Unlike wired networks, which require physical access, wireless networks broadcast data over the air, making them more susceptible to attacks.

---

## Objective: 
To understand the fundamentals of wireless network security, common vulnerabilities associated with wireless technologies, and best practices for securing wireless networks.

---

## 1. Introduction to Wireless Networks
### Overview of Wireless Networks:
Wireless networks (Wi-Fi) use radio waves to transmit data, enabling devices to communicate without physical connections. They are convenient for mobility but can be vulnerable to various types of attacks, making security crucial.
Wireless networks can be categorized into WLANs (Wireless Local Area Networks), WANs (Wide Area Networks), and personal networks (like Bluetooth).

---

## Common Wireless Network Standards:
1. 802.11 is the most common standard for Wi-Fi networks. It has gone through multiple iterations
- 802.11b/g/n (older standards, now less secure).
- 802.11ac/ax (modern standards, offering faster speeds and better security features).

### Wireless Network Vulnerabilities:
1. Weak Encryption: Older encryption standards like WEP (Wired Equivalent Privacy) are highly insecure. Modern networks should use WPA2 (Wi-Fi Protected Access 2) or WPA3, which are much stronger.

2. Weak Passwords: Weak or default passwords on Wi-Fi routers can allow attackers to easily gain access to the network.

3. Rogue Access Points: Attackers can set up unauthorized access points that mimic legitimate networks, tricking users into connecting to them (called Evil Twin attacks).

---

## 2. Securing Wireless Networks
### Securing Wireless Networks:
1. Encryption:
- Use the strongest encryption available. WPA2 (AES encryption) and WPA3 are the most secure encryption standards for protecting wireless data. Avoid WEP as it is easily cracked by attackers.

2. Strong Passwords:
Always set strong, complex passwords for your Wi-Fi. Passwords should be long (at least 12-16 characters) and include a mix of upper/lowercase letters, numbers, and special characters.

3. Disable WPS (Wi-Fi Protected Setup):
WPS is a feature that allows users to easily connect devices to a Wi-Fi network by pressing a button on the router. However, it is vulnerable to brute force attacks, so it’s safer to disable it.

4. SSID (Service Set Identifier) Management:
Change the default SSID to something unique to avoid making your network easily identifiable. Also, consider disabling SSID broadcasting so that your network won’t appear in available network lists (making it harder for attackers to target).

5. MAC Address Filtering:
Limit which devices can connect to your network by allowing only specific MAC addresses (unique hardware addresses) to join the network. This adds an additional layer of control, but it is not foolproof, as MAC addresses can be spoofed.

6. Router Placement:
Place wireless routers in the center of the house or office to limit the signal's reach outside of the building. This reduces the risk of external attackers accessing your network.

7. Monitoring Wireless Networks:
- Regularly monitor the network for unauthorized devices and unusual traffic patterns. Tools like Wireshark or NetSpot can help identify rogue devices and suspicious activity.
- Intrusion Detection Systems (IDS): Use IDS to detect and respond to potential security incidents in real-time.

8. Protecting against Common Wireless Attacks:
- Evil Twin Attacks: Avoid falling victim to rogue access points by ensuring that your devices only connect to known and trusted SSIDs.

- Deauthentication Attacks: This attack disconnects devices from the network by sending deauthentication frames. Implement 802.11w (management frame protection) to defend against this type of attack.

- Denial of Service (DoS): Protect the network against flooding attacks by limiting the number of devices that can connect to the network and monitoring traffic for abnormal patterns.

---

## Today's Learning Summary:
- Today’s session gave me a solid understanding of the potential risks and vulnerabilities associated with wireless networks. I now understand how to secure a wireless network by using strong encryption (WPA2/WPA3), setting complex passwords, disabling unnecessary features like WPS, and employing strategies like SSID management and MAC address filtering.
- I also learned about common wireless attacks such as Evil Twin and Deauthentication attacks, and how to defend against them with best practices like using encryption, monitoring network traffic, and placing routers strategically.
- The session ended with a discussion on the risks of using public Wi-Fi networks, which are often unsecured. We learned how to use VPNs to protect data transmitted over public Wi-Fi and the importance of avoiding sensitive activities, like online banking, when connected to an unsecured network.
