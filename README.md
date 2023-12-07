# # Incident Final Report

## Executive Summary

The organization encountered a security incident on December 28, 2022, at 7:20 p.m., PT, wherein an unauthorized individual gained access to customer personal identifiable information (PII) and financial details. Approximately 50,000 customer records were impacted, resulting in an estimated $100,000 in direct costs and potential revenue loss. The incident has been resolved, and a comprehensive investigation has been conducted.

## Timeline

- **December 22, 2022 (3:13 p.m., PT):** An employee received an email from an external source claiming successful theft of customer data, demanding a $25,000 cryptocurrency payment. The employee treated it as spam and deleted the email.
  
- **December 28, 2022:** The same employee received a second email from the same sender, including a sample of stolen data and an increased payment demand of $50,000.

- **December 28 - December 31, 2022:** The security team initiated an investigation to determine the data theft methods and extent.

## Investigation

- The security team identified the root cause as a vulnerability in the e-commerce web application, enabling a forced browsing attack.
  
- The attacker manipulated order numbers in the URL string of a purchase confirmation page, accessing and exfiltrating customer transaction data.

- Examination of web application access logs revealed the attacker accessed information from thousands of purchase confirmation pages.

## Response and Remediation

- The organization collaborated with the public relations department to disclose the breach to customers.
  
- Free identity protection services were offered to affected customers.
  
- Web server logs analysis confirmed the attack source: a single log displaying an exceptionally high volume of sequentially listed customer orders.

## Recommendations

To prevent future incidents, the following actions are being taken:

1. **Routine Scans and Testing:**
   - Conduct regular vulnerability scans and penetration testing to identify and address potential security weaknesses.

2. **Access Control Mechanisms:**
   - Implement allowlisting to restrict access to a specified set of URLs, automatically blocking requests outside this range.
  
   - Ensure that only authenticated users have authorized access to content.

These measures aim to enhance the organization's security posture and mitigate the risk of similar incidents in the future.
