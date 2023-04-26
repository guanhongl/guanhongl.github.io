---
layout: project
type: project
image: img/minerva/minerva-square.png
title: "Minerva"
date: 2022-09
published: true
labels:
  - Meteor
  - Meteor Cloud
  - React
  - MongoDB
summary: "An electronic inventory management system for a nonprofit clinic."
---

<img class="img-fluid" src="../img/minerva/minerva-home-page.png">

[Visit Website](https://minerva.meteorapp.com/)  
[Visit GitHub Repo](https://github.com/guanhongl/minerva-matrp)  
[Visit Clinic Website](https://sites.google.com/view/hawaiihomeproject/about)  

## What is Hawaii H.O.M.E. Clinic?

Hawaii Homeless Outreach & Medical Education (H.O.M.E.) Clinic is a mobile clinic that sees patients at various sites around the island. The mission is to improve access to health care for the houseless while understanding their healthcare needs. 

## The Problem

The clinic used Athenahealth Electronic Health Record (EHR) to document ordered drugs and vaccines at the end of an encounter and a Google Forms & Sheets system to log and deduct drugs and vaccines from the master inventory. Manually entering information proved to be a pain point; the process was slow and the supply was inaccurate. It was difficult for the business to manage their supply. **The clinic needed an inventory management system!** 

The problem was introduced to me during my Software Engineering II course. My team of 8 worked in short sprints with regular communication and using GitHub Project Boards and Issues for agile project management. The app was largely incomplete by the course end, thus, I volunteered to continue and push it to production. 

## Saving Time, Saving Resources

The proposed solution was to replace the Google Forms & Sheets system with an inventory management app that applies QR codes to each batch of drugs and vaccines. A QR code links to an item's lot number which uniquely identifies the batch of product produced by a manufacturer. Scanning a QR code opens the item's information page. And on the page are links to the add and dispense forms auto-populated with the item's information. Once complete, a log of the transaction is stored and the master inventory is updated. The improved business process provides physicians with numerous benefits. 

- They save time by not having to manually enter information
- Inventory quantities are accurate due to QR code and database integrity
- They can easily access inventory and log information via searches and filters
- They are notified when supply is low or nearing expiration in real-time

The app is built with Meteor, a full-stack JavaScript framework that bundles React, MongoDB, and Node.js, and hosted with Meteor Cloud. 

<div class="container text-center">
  <div class="row">
    <div class="col">
      <img src="../img/minerva/minerva-qr-code.png" class="img-fluid">
    </div>
    <div class="col">
      <img src="../img/minerva/minerva-log-page.png" class="img-fluid">
    </div>
  </div>
</div>

## Integrating Athenahealth APIs

Athenahealth EHR continued to document ordered, administered or dispensed, drugs and vaccines for patients at the end of an encounter. To further save time, I proposed a pipeline to fetch ordered drug and vaccine information for the day to sync to the database; ordered drug and vaccine quantities are auto deducted from the master inventory at night. I coordinated with the EHR vendor to gain API access and design the data pipeline. Using Athenahealth's [Changed Data Subscriptions](https://docs.athenahealth.com/api/guides/changed-data-subscriptions) the app can subscribe to the changed orders feed and fetch the created orders for the day. 

- Drugs and vaccines administered or dispensed on Athenahealth are auto deducted from the app's inventory
- They save time by not having to dispense on the app
- No personal identifiable information is stored on the app

## Results

Due to the new app, the required effort for adding and dispensing supply was reduced. Managing supply was easier, as inventory and log information was structured, which meant happier physicians. 

I learned to adapt my solution to the client's request. Understanding the client's business process is crucial! I often had to clarify details and rework solutions as new information arrived. What I found most helpful was visiting the clinic and chatting in person. 

## More on Meteor


