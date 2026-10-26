# Task Hub

Task Hub is a custom document intake and workflow automation platform designed to streamline how a professional services firm receives, processes, organizes, and manages client documents.

## Overview

The system integrates with Microsoft 365 to automatically retrieve incoming documents, identify relevant information, match documents to client records, and route files to the appropriate directories.

Documents that cannot be confidently processed are flagged for human review.

## Problem

Professional services firms often receive large volumes of client documents through email. Manually identifying, categorizing, and filing these documents is time-consuming and introduces opportunities for errors.

Task Hub was developed to reduce repetitive administrative work while maintaining visibility and control over document handling.

## Solution

Task Hub automates key stages of document processing, including:

- Email ingestion through Microsoft Graph
- PDF extraction and document classification
- Client and document-type identification
- Payer-specific checklist matching
- Automated routing to client directories
- Human review of ambiguous documents
- Role-based access control and user permissions
- Error handling and recoverable file operations

## System Architecture

Microsoft 365 Mailboxes  
↓  
Microsoft Graph API  
↓  
Python / Flask Application  
↓  
Document Extraction & Classification  
↓  
Client Matching & Routing  
↓  
Network File Storage / Human Review

## Tech Stack

- Python
- Flask
- SQLite
- Microsoft Graph API
- Microsoft Authentication Library (MSAL)
- OAuth 2.0
- PyMuPDF / pypdf
- Windows Network Storage
- pytest

## Engineering Highlights

### Security

Implemented role-based access control across four staff roles and 25 capabilities, including route-level authorization, scoped data access, and CSRF protection.

### Reliability

Developed recoverable file operations and addressed email-processing and cross-platform PDF extraction issues to improve system reliability.

### Testing

Developed and maintained a test suite containing 586 automated tests, verified on macOS and Windows.

## My Contribution

I independently led the software engineering work, including:

- System architecture and technical design
- Backend application development
- Microsoft Graph and authentication integrations
- Document processing and workflow automation
- Database design and access controls
- Automated testing and debugging
- Deployment preparation and technical troubleshooting

## Project Status

Task Hub is currently running in a pre-pilot environment connected to the firm's infrastructure. Broader staff rollout has not yet occurred.

## Code Availability

Task Hub was developed for a private client. The source code, client information, and internal configurations are not publicly available.

This repository provides a high-level overview of the system and the engineering work involved.
