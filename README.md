# Tamper Proof Data

At Bequest, we require that important user data is tamper proof. Otherwise, our system can incorrectly distribute assets if our internal server or database is breached. 

**1. How does the client ensure that their data has not been tampered with?**

- Digital Signatures: Employ cryptographic seals to certify data. This guarantees detection of any data alteration, as the seal will become invalid.
- Hash Functions:  Store data fingerprints (hash values). When retrieving data, recalculate the fingerprint and compare it to the stored one. A match confirms the data's authenticity.
- Blockchain Technology: Utilize blockchain for data storage. Blockchain safeguards data integrity through its distributed, unalterable ledger system.
- Audit Logs: Maintain unchangeable audit logs that track all data actions. These logs should be tamper-proof and offer a comprehensive history of modifications.

- Safeguarding Data Access and Activity
  - RBAC / Role-Based Access Control: Restrict data access and modification to authorized users only. This approach minimizes the chance of unauthorized alterations.
  - IDS / Intrusion Detection Systems: Implement IDS to continuously monitor for suspicious activity that might signal data tampering attempts. The system will then alert relevant personnel.
  - Regular Security Assessments: Conduct periodic security audits and penetration testing to proactively identify and address potential vulnerabilities before they can be exploited.

<br />
**2. If the data has been tampered with, how can the client recover the lost data?**

- Data Backup Strategies:
  - Scheduled Backups:  Establish consistent backup routines (daily, weekly, monthly) and guarantee backups are securely stored in various locations.
  - Data Versioning: Maintain historical copies of your data. This allows you to rollback to a previous, uncorrupted version if tampering occurs.
  - Unalterable Backups: Store backups in a format that cannot be modified, preventing tampering of the backup data itself.

- Data Recovery Procedures:
  - Automated Recovery:  Develop automated processes for swift data restoration from backups. This minimizes disruption in case of data tampering incidents.
  - Disaster Recovery Plan:  Craft and maintain a detailed disaster recovery plan outlining the steps to take in case of data loss or corruption.
  - Backup Verification:  Regularly test backup restoration procedures to ensure data can be recovered effectively and without problems.

### To run the apps:
```npm run start``` in both the frontend and backend

## To make a submission:
1. Clone the repo
2. Make a PR with your changes in your repo
3. Email your github repository to robert@bequest.finance
