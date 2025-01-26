# Projektni zadatak RCA - Portfolio

## Overview

This project simulates a personal cryptocurrency portfolio, allowing users to track their cryptocurrency holdings, profits, and losses in real-time. It features a web application for user interaction, worker roles for notifications and health monitoring, and integration with external APIs for cryptocurrency values.

---

## Features
### PortfolioService (Web Role)
1. User registration.  
2. Login via email and password.  
3. Portfolio management:
   - Add cryptocurrency purchase/sale records.
   - Delete transactions.
   - Display profit/loss per cryptocurrency and total portfolio value.
4. Cryptocurrency search.  
5. Integration with Binance API for cryptocurrency values.  

---

## Services
### NotificationService
- Sends email notifications when a profit threshold for a cryptocurrency is exceeded.  
- 3 instances, processing up to 20 alerts every 10 seconds.  
- Emails are sent using **MailKit.Net.Smtp**.  

### HealthMonitoringService
- Checks system availability every 1-5 seconds.  
- Logs results into the `HealthCheck` table.  

### HealthStatusService
- Provides a visual representation of service availability and uptime statistics.  

---

## Technologies
- **Cloud Platform**: Microsoft Azure Cloud Services  
- **Backend**: .NET (Azure Web and Worker Roles)  
- **Frontend**: MVC web application  
- **Database**: Azure Table and Blob Storage

---

## Authors
- ArsenijeKnez
- dragangavric01
- BojanKuljic
- lukaispanovic
