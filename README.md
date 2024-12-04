# SafetyNet Alerts System

**SafetyNet Alerts** is a Spring Boot application designed to deliver essential information related to fire stations, emergency notifications, and community data. This platform provides RESTful APIs for retrieving details about individuals, fire stations, and community contacts based on specific criteria.

---

## Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [System Architecture](#system-architecture)
4. [Technology Stack](#technology-stack)
5. [Setup and Installation](#setup-and-installation)
6. [How to Run](#how-to-run)
7. [API Documentation](#api-documentation)
   - [Retrieve People by Fire Station](#retrieve-people-by-fire-station)
   - [Child Residence Alert](#child-residence-alert)
   - [Emergency Contact Numbers](#emergency-contact-numbers)
   - [Fire Incident Details](#fire-incident-details)
   - [Flood Readiness Alerts](#flood-readiness-alerts)
   - [Detailed Personal Information](#detailed-personal-information)
   - [Citywide Email Directory](#citywide-email-directory)
8. [Testing](#testing)
9. [Logging](#logging)
10. [Contributions](#contributions)
11. [License](#license)

---

## Overview

**SafetyNet Alerts** streamlines access to critical safety information, providing users with a suite of tools to manage fire station data, generate alerts, and enhance community preparedness.

---

## Features

- **Fire Station Coverage**: Fetch a list of individuals served by specified fire stations.
- **Children Alerts**: Identify children living at a particular address and include details of their household members.
- **Emergency Phone Directory**: Retrieve phone numbers of residents within a fire station's operational area.
- **Fire Response Data**: Access detailed information about residents at a specific location, including medical histories.
- **Flood Response Planning**: Categorize households by fire station jurisdiction for flood preparation.
- **Individual Profiles**: Look up detailed personal records using a first and last name combination.
- **City Email Collection**: Compile email addresses for all residents in a specific city.
- **Detailed Logging**: Log all incoming requests and outgoing responses for auditing and troubleshooting.
- **Reliable Testing**: Extensive unit tests verify functionality and prevent regressions.
- **Scalable Design**: Built with the MVC architecture, adhering to SOLID principles for maintainability.

---

## System Architecture

SafetyNet Alerts employs a **Model-View-Controller (MVC)** architecture:

- **Model**: Represents the core data entities such as `Person` and `FireStation`. Handles database interaction via repositories.
- **Controller**: Processes client HTTP requests, interacts with service layers, and delivers appropriate HTTP responses.
- **Service**: Implements business logic by manipulating and preparing data for the controllers.
- **View**: Provides RESTful API endpoints for seamless client communication.

---

## Technology Stack

- **Programming Language**: Java 17
- **Frameworks**: 
  - Spring Boot
  - Spring Web
  - Spring Data JPA
- **Database**: H2 Database (configurable for other relational databases)
- **Build Tool**: Maven
- **Testing**: JUnit and Mockito
- **Logging**: SLF4J with Logback

---

## Setup and Installation

1. Clone the project repository:

   ```bash
   git clone https://github.com/Fall2024-NSCC-ECampus/final-project-alerts-notification-system-w0140158.git
   cd final-project-alerts-notification-system-w0140158
