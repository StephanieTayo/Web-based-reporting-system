# Web-based reporting system

# Brief Overview

This document provides comprehensive documentation for the software. It covers various aspects such as installation, configuration, usage, testing, and more.

# Objective

## Purpose and Goals

The primary purpose of the software is to generate a simplified report from provided data for client presentation. Goals include creating a professional, client-friendly report in PDF format with interactive elements and implementing an automated pipeline for parsing arbitrary databases.

# Project Overview

## Project Scope and Boundaries

The project encompasses the development of a web application that generates client-friendly reports from structured data. It includes the parsing of CSV data, report generation in PDF format, and an interactive user interface.

## Target Audience or Users

The software is designed for clients who require simplified reports derived from structured data. The target audience includes non-technical users who need an easily understandable representation of data.

# System Architecture

## Component Relationships and Interactions

The system consists of components for data parsing, report generation, and a web server. Interaction occurs between the user interface, data parsing components, and the reporting module.

## Deployment Architecture

The software is deployed as a web application accessible through a web server. The application components are hosted on a server infrastructure.

## Technical Stack

Technologies, Frameworks, and Languages Used <br>
Node.js for server-side development <br>
Express.js for web application framework <br>
EJS for templating <br>
PDF generation library, html2pdf <br>
Jest for Functional Unit testing <br>

## Version Information for Key Components

Node.js version v18.14.2

Express.js version ^4.18.2

csv-parser ^3.0.0

## Installation Guide

Step-by-Step Instructions

Clone the repository.

Install Node.js and npm.

Install project dependencies using npm install.

Start the project with npm start

# Usage Guide

## Instructions on How to Use the Software

Access the web application through a browser.

Upload CSV files in data folder for data parsing.

# Code Documentation

## Inline Comments

For example;

// generates HTML table for department data

function generateTable(departments, counter)

# Testing

## Test Cases and Scenarios

1. CSV Parsing

Scenario ; Checks if it correctly parses CSV file into JavaScript objects

2. Read Directories

Scenario ; Checks if it correctly reads directory structure and finds CSV files

3. Sanitize DirKey

Scenario 1 ; Should normalize Windows path separators to Unix-like

Scenario 2 ; Should remove leading current directory indicator "./"

Scenario 3 ; Should remove leading parent directory indicator "../"

Scenario 4 ; Should remove "data/" prefix if present

...

4. App Routes

Scenario ; Should render the index view with the correct data

# Testing Tools and Methodologies Used

Jest - Used for unit testing individual functions and components. This was selected as it provides a simple and fast testing framework for javascript applications.

To test run; npm test
