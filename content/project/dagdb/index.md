---
title: DataArmorGate DB (Gate DB)
summary: A database proxy application that enables users to perform SQL queries on encrypted data without storing the key to the database server. 
tags:
- Work
date: "2019-11-11T00:00:00Z"

# Optional external URL for project (replaces project detail page).
# external_link: "https://www.linkedin.com/products/eaglys-inc.-dataarmor-gate-db/"

image:
  caption: DataArmorGate DB
  focal_point: Smart

links:
- icon: linkedin
  icon_pack: fab
  name: Gate DB
  url: https://www.linkedin.com/products/eaglys-inc.-dataarmor-gate-db/
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example 
---
DataArmor Gate DB is a turn key solution for always-on encryption of databases that contain highly sensitive data or operate in non-trusted zones such as the cloud. The contents of the database are always encrypted and all queries are performed over encrypted data only. The encryption keys are stored separately from the database, and data is never decrypted at the database side. This is in contrast to current database solutions which partially decrypt the data when performing queries.
### Notable features of Gate DB:

- data is always-on encryption(during communication, at rest, during processing).
- The contents of the database are always encrypted and all queries are performed over encrypted data.
- The encryption keys are not stored in the database.
- It supports bring-your-own-key(BIOK)
- data is never decrypted at the database side which is different from traditional database systems.
  
### Key contributions:
  - Implemented Homomorphic-encryption(HE) to perform ‘SQL aggregate functions’.
  - Reduced the bulk insertion and encryption time by 5 times by eﬀicient implementation of HE algorithms and multi-processing in Rust.
  - Implemented Lifted-ElGamal over prime field as Somewhat-Homomorphic-Encryption (using BLS-12 elliptic curve pairing) for Homomorphic addition of cipher-text.
  - Improved the bulk data transmission using gRPC between client and the proxy.