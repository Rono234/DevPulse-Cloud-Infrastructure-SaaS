# DevPulse-Cloud-Infrastructure-SaaS
CSI_3150 Assignment 1_b coding part

**Author:** Raneen AlRammahi  
**Course:** CSI-3150  
**Date:** September 20, 2026  

# Section 1: The Less-than-or-Equal-to-4-Click User Journey Funnel

- **Starting State:**  
  The user lands on the DevPulse homepage. The initial viewport displays the DevPulse branding, primary navigation links, core platform value proposition/metrics, and a prominent "Deploy Free Cluster" call-to-action.

- **Action 1:**  
  The user scrolls or selects the "Pricing" navigation link to move directly to the tier comparison section.

- **Action 2:**  
  The user reviews the Developer, Pro Cluster, and Enterprise Dedicated plans and selects the appropriate tier, such as "Pro Cluster."

- **Action 3:**  
  The user enters the expected node count and log throughput into the constrained workload estimator and reviews whether the selected tier supports the workload.

- **Action 4:**  
  The user completes the API provisioning registration form and activates the registration submission button.

- **Terminal State:**  
  The browser displays confirmation feedback indicating that the registration request was successfully submitted and that API sandbox provisioning information will be provided.


# Section 3: Semantic Component & Layout Tree

```text
index.html
│
├── <body>
│   │
│   ├── <header>
│   │   ├── <a href="#">
│   │   │   └── DevPulse Logo / Home
│   │   │
│   │   └── <nav> — Primary Navigation
│   │       ├── <a href="#features">
│   │       │   └── "Features"
│   │       ├── <a href="#pricing">
│   │       │   └── "Pricing"
│   │       ├── <a href="#workload">
│   │       │   └── "Workload Estimator"
│   │       ├── <a href="#api-registration">
│   │       │   └── "API Registration"
│   │       └── <a href="#api-registration">
│   │           └── "Deploy Free Cluster" — Primary CTA
│   │
│   ├── <main>
│   │   │
│   │   ├── <section id="hero">
│   │   │   ├── <img>
│   │   │   │   └── DevPulse Infrastructure Graphic
│   │   │   ├── <h1>
│   │   │   │   └── "DevPulse Cloud Infrastructure"
│   │   │   ├── <p>
│   │   │   │   └── Primary Value Proposition
│   │   │   └── <nav> — Hero CTA Group
│   │   │       ├── <a href="#pricing">
│   │   │       │   └── "View Pricing"
│   │   │       └── <a href="#api-registration">
│   │   │           └── "Get API Keys"
│   │   │
│   │   ├── <section id="features">
│   │   │   ├── <header>
│   │   │   │   ├── <h2>
│   │   │   │   │   └── "Platform Capabilities"
│   │   │   │   └── <p>
│   │   │   │       └── Section Subheading
│   │   │   │
│   │   │   ├── <article>
│   │   │   │   ├── <h3>
│   │   │   │   │   └── "Latency Tracking"
│   │   │   │   └── <p>
│   │   │   │       └── Feature Description
│   │   │   │
│   │   │   ├── <article>
│   │   │   │   ├── <h3>
│   │   │   │   │   └── "Log Aggregation"
│   │   │   │   └── <p>
│   │   │   │       └── Feature Description
│   │   │   │
│   │   │   └── <article>
│   │   │       ├── <h3>
│   │   │       │   └── "Auto-Remediation"
│   │   │       └── <p>
│   │   │           └── Feature Description
│   │   │
│   │   ├── <section id="pricing">
│   │   │   ├── <header>
│   │   │   │   ├── <h2>
│   │   │   │   │   └── "Compute Tier Comparison"
│   │   │   │   └── <p>
│   │   │   │       └── Section Subheading
│   │   │   │
│   │   │   ├── <article>
│   │   │   │   ├── <h3>
│   │   │   │   │   └── "Developer"
│   │   │   │   ├── <p>
│   │   │   │   │   └── Plan Description
│   │   │   │   └── <ul>
│   │   │   │       ├── <li> — Feature
│   │   │   │       └── <li> — Feature
│   │   │   │
│   │   │   ├── <article>
│   │   │   │   ├── <strong>
│   │   │   │   │   └── "Most Popular"
│   │   │   │   ├── <h3>
│   │   │   │   │   └── "Pro Cluster"
│   │   │   │   ├── <p>
│   │   │   │   │   └── Plan Description
│   │   │   │   └── <ul>
│   │   │   │       ├── <li> — Feature
│   │   │   │       └── <li> — Feature
│   │   │   │
│   │   │   └── <article>
│   │   │       ├── <h3>
│   │   │       │   └── "Enterprise Dedicated"
│   │   │       ├── <p>
│   │   │       │   └── Plan Description
│   │   │       └── <ul>
│   │   │           ├── <li> — Feature
│   │   │           └── <li> — Feature
│   │   │
│   │   ├── <section id="workload">
│   │   │   ├── <header>
│   │   │   │   ├── <h2>
│   │   │   │   │   └── "Workload Estimator"
│   │   │   │   └── <p>
│   │   │   │       └── Section Subheading
│   │   │   │
│   │   │   └── <form>
│   │   │       ├── <fieldset>
│   │   │       │   ├── <legend>
│   │   │       │   │   └── "Infrastructure Workload Requirements"
│   │   │       │   │
│   │   │       │   ├── <label for="node-count">
│   │   │       │   │   └── "Node Count"
│   │   │       │   │
│   │   │       │   ├── <input>
│   │   │       │   │   ├── id="node-count"
│   │   │       │   │   ├── name="node-count"
│   │   │       │   │   ├── type="number"
│   │   │       │   │   ├── min="1"
│   │   │       │   │   ├── max="1000"
│   │   │       │   │   ├── step="1"
│   │   │       │   │   └── required
│   │   │       │   │
│   │   │       │   ├── <small>
│   │   │       │   │   └── "Minimum 1 - Maximum 1000"
│   │   │       │   │
│   │   │       │   ├── <label for="log-throughput">
│   │   │       │   │   └── "Log Throughput"
│   │   │       │   │
│   │   │       │   ├── <input>
│   │   │       │   │   ├── id="log-throughput"
│   │   │       │   │   ├── name="log-throughput"
│   │   │       │   │   ├── type="number"
│   │   │       │   │   ├── min="1"
│   │   │       │   │   ├── max="10000"
│   │   │       │   │   ├── step="1"
│   │   │       │   │   └── required
│   │   │       │   │
│   │   │       │   └── <small>
│   │   │       │       └── "Minimum 1 - Maximum 10000 GB/day"
│   │   │       │
│   │   │       └── <button type="submit">
│   │   │           └── "Check Tier Compatibility"
│   │   │
│   │   └── <section id="api-registration">
│   │       ├── <header>
│   │       │   ├── <h2>
│   │       │   │   └── "API Sandbox Registration"
│   │       │   └── <p>
│   │       │       └── Section Subheading
│   │       │
│   │       └── <form>
│   │           ├── <fieldset>
│   │           │   ├── <legend>
│   │           │   │   └── "Developer Contact Information"
│   │           │   │
│   │           │   ├── <label for="first-name">
│   │           │   │   └── "First Name"
│   │           │   │
│   │           │   ├── <input>
│   │           │   │   ├── id="first-name"
│   │           │   │   ├── name="first-name"
│   │           │   │   ├── type="text"
│   │           │   │   └── required
│   │           │   │
│   │           │   ├── <label for="last-name">
│   │           │   │   └── "Last Name"
│   │           │   │
│   │           │   ├── <input>
│   │           │   │   ├── id="last-name"
│   │           │   │   ├── name="last-name"
│   │           │   │   ├── type="text"
│   │           │   │   └── required
│   │           │   │
│   │           │   ├── <label for="work-email">
│   │           │   │   └── "Work Email"
│   │           │   │
│   │           │   ├── <input>
│   │           │   │   ├── id="work-email"
│   │           │   │   ├── name="work-email"
│   │           │   │   ├── type="email"
│   │           │   │   └── required
│   │           │   │
│   │           │   ├── <label for="tier">
│   │           │   │   └── "Cluster Tier"
│   │           │   │
│   │           │   └── <select>
│   │           │       ├── id="tier"
│   │           │       ├── name="tier"
│   │           │       ├── required
│   │           │       ├── <option value="">
│   │           │       │   └── "Select a Tier"
│   │           │       ├── <option value="developer">
│   │           │       │   └── "Developer"
│   │           │       ├── <option value="pro">
│   │           │       │   └── "Pro Cluster"
│   │           │       └── <option value="enterprise">
│   │           │           └── "Enterprise Dedicated"
│   │           │
│   │           └── <button type="submit">
│   │               └── "Request API Sandbox"
│   │
│   └── <footer>
│       ├── <p>
│       │   └── "© 2026 DevPulse Cloud Infrastructure"
│       │
│       └── <nav> — Footer Navigation
│           └── <ul>
│               ├── <li>
│               │   └── <a href="#features">
│               │       └── "Features"
│               ├── <li>
│               │   └── <a href="#pricing">
│               │       └── "Pricing"
│               ├── <li>
│               │   └── <a href="#workload">
│               │       └── "Workload Estimator"
│               ├── <li>
│               │   └── <a href="#api-registration">
│               │       └── "API Registration"
│               └── <li>
│                   └── <a href="#">
│                       └── "Back to Top"
```

