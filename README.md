# SwasthyaChain-BlockChain-Based-Health-Management-System
The project aims to use blockchain technology to create a user-focused electronic health
record whilst maintaining a single true version of the user’s data.Swasthya Mitra is a
decentralised platform that enables secure, fast and transparent exchange and usage of
medical data.
Swasthya Mitra will enable users to give conditional access to different healthcare agents
such as doctors, hospitals, laboratories, pharmacists and insurers to interact as they see fit.
Each interaction with their medical data is auditable, transparent and secure, and will be
recorded as a transaction on Swasthya Mitra distributed ledger. During this process, the
patient’s privacy is protected at all times. Swasthya Mitra is built on the permission-based
Hyperledger Fabric architecture which allows varying access levels; users control who can
view their records, how much they see and for what length of time. By empowering users,
we can build the future of healthcare together. Swasthya Mitra will be a platform for other
digital health applications to develop on; users will be able to sign for these applications
and services which are powered by their health data and secured by smart contracts.
# Swasthya Mitra Solution ​: The Healthcare of Tomorrow
● Dual Blockchain: Swasthya Mitra is built using a dual blockchain structure. The first
blockchain controls access to health records and is built using Hyperledger Fabric.
The second blockchain is powered by an ERC20 token on Ethereum and underlies
all the applications and services for our platform.
● The Hyperledger blockchain network is permission-based and requires users to sign
up to use it. Permissioning on the network is controlled using Hyperledger modelling
and access control languages. Hyperledger Fabric is a platform for distributed ledger
solutions underpinned by a modular architecture delivering high degrees of
confidentiality, resilience, flexibility and scalability.
Working of the Network
Participants Involved
1. Practitioner
a. Read/Write on permissioned EHRs
b. Request permission for other Practitioner/ Institutions to gain Read/Write
access
2. Patient
a. Read their EHR
b. Permission a Practitioner/Institution to Read/Write EHR or a portion of their
EHR
c. Revoke permission from Practitioners/Institutions
d. Permission next of kin/emergency contact to Read/Grant permission
e. Write certain attributes to EHR
i. Amount of tobacco consumed daily
ii. Alcohol consumed weekly
iii. Weekly exercise
f. Ability to integrate IoT data into EHR
Encryption Scheme
To ensure privacy, health records are encrypted using symmetric key cryptography. The
record will be encrypted and stored in a data store within the appropriate regulatory
jurisdiction. The symmetric key will be encrypted with the public key of a 2048-bit RSA key
pair.
Transactions
Any interactions with health records are recorded as transactions on the network. To
ensure privacy, health records are encrypted using symmetric key cryptography.
Transactions are viewable only to the participants associated with the transaction.
Every patient and practitioner would have its own asset which could only be accessed by
the individual himself.
There would be 3 types of transactions:
1. Patient Granting Access
2. Patient Revoking Access
3. Practitioner Referring Patient
Patient Granting Access
● Patient A grants access to EHR to Practitioner A
● Practitioner A’s ID is added to Patient A’s authorised asset on the ledger
● Patient A’s ID is added to Practitioner A’s authorised asset on the ledger
● The Symmetric key for the EHR is decrypted with Patient A’s private key
● Symmetric key is then encrypted with Practitioner A’s public key
Patient Revoking Access
● Practitioner A’s ID is removed from Patient A’s authorised asset
● Patient A’s ID is removed from Practitioner A’s authorised asset
● Patient A’s private key is used to decrypt Symmetric key for EHR which is
used to decrypt the EHR
● The new Symmetric key of EHR is encrypted with Patient A’s public key and
the public keys of all the remaining IDs that have permission
Practitioner referring Patient
● Practitioner A updates the permissions to allow Practitioner B to access the
Patient’s EHR.
● Chaincode will check that Practitioner A has permission on the EHR.
● Practitioner A uses its private key to decrypt the EHR’s symmetric key
● Practitioner B’s public key is used to encrypt the Symmetric key
● Practitioner B’s ID is added to Patient A’s authorised asset
● Patient A’s ID is added to Practitioner B’s authorised asset

We plan to build a common platform accessible to citizens, hospitals and the
government. Under this, there would be a digital Health Card for each and every citizen
of Chhattisgarh. Health Card will be unique to each individual as it would be based on
Aadhar​ Identity. The government can use it to design better health schemes in
effective manner. As the Govt, would get the real time data of health condition.
A web app​ that allows the (i) citizen to view his organised medical history, prescription,
test results, ongoing treatments and medications (ii) the doctors to edit their treatment
history and add prescriptions, medications, referrals, tests and results and view their
patient's’ history. (iii) The government to view the analysis and schematics (past,
present and predictions) of a region, to help them identify problem areas and launch
successful schemes and programmes.

1. BENEFITS FOR GOVERNMENT
1.1 Data Science : Using the health data of every person , we would provide healthcare
inferences to the government.Government can use it to design better health schemes
in effective manner. Area specific schemes
1.2 AI : Based on the data from Chhattisgarh and similar data from all over the world ,
we can predict any health complications in any area . It could help to prevent epidemic
breakout.
1.3 It could help government to prevent delays in the Treatment as it would have Real
time data from all over the state. I.e. thereby removing corruption and delays in
healthcare.
1.4 Send notifications for ongoing health problems in the area and also for vaccinations
of child.

2. BENEFITS FOR AN INDIVIDUAL/CITIZENS
2.1 The entire health history of a person would be stored which would be reflected in
the Person’s Digital Health Card.
2.2 Now no need to carry all previous prescriptions , any doctor can directly see the
health card of that person and recommend the solutions based on that and it would be
very effective
2.3 Person living in remote villages can directly call the health expert and get all expert
solutions based on his UID.
2.4 Appointment booking
2.5 All DBT related to healthcare would be directly transferred to that account.
2.6 Newly born babies would be enrolled in and their vaccination schedule could be
tracked and regular and timely notification for vaccines can be provided

3. BENEFITS FOR HOSPITALS/DOCTORS
3.1 Doctors would have all previous data of the concerned patient & it can help the
doctor to better predict the disease.
3.2 Hospital can better manage the medicine stock.

# A Better System
● User Control
  ○ In the current healthcare system, patients have their health information
spread over multiple systems, hospitals, networks and potentially countries.
There are multiple fragmented records from the same patient, held at
different institutions all with their own snapshot of the patient’s health at the
point of their interaction with them, such as blood tests, imaging and clinic
letters. Swasthya Mitra will chronologically arrange all of these records and
filter them into the specific categories above to aid data handling. Such a
categorisation would make the records more accessible and understandable
for patients and it will also facilitate researchers in searching for the
information relevant to them

● Data Security
  ○ The Swasthya Mitra system uses a double encryption mechanism on a
closed, permission-based blockchain. The security of health records is
secured beyond any centralised data system currently in use. Patient data is
not accessible directly on the blockchain. The blockchain acts as a pointer to
where patient data is held in an encrypted format, meaning that anyone
attempting to intercept patient data will be unable to with the ease that is
required to access data existing in any central location.

● Clinical Communication
  ○ Along with increased access to emergency information, Swasthya Mitra
allows clinicians to communicate with each other with ease. When an
authorised healthcare professional updates a patient health record, the
system will update that record on Swasthya Mitra . Any clinician with
authorised access to that record will see the update in real time. As health
records are updated via Swasthya Mitra for all authorised parties, there is no
need for patient data to be manually transferred from system to system.
Swasthya Mitra will be usable in any browser on any computer. As a result,
any doctor with a browser and an internet connection will be able to access
the users’ documents shared with them. Issues currently associated with
interoperability are resolved this way and costs that are associated with the
transportation of notes currently undertaken by junior clinicians or
administrative staff are cut down on.

