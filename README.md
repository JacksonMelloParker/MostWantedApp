Group Project - README Template
===

# MWA

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description
An app for users to look up the most wanted criminals in the US.

### App Evaluation
- **Category:** Security
- **Mobile:** This app would be mainly used on mobile devices since officer will be using it in the daily basis.
- **Story:** Display monst wanted people on the FBI list and give the option to search a name in the list.
- **Market:** Police officer could use this app to look up and search people in the most wanted list.
- **Habit:** This app could be used by police officers to check if possible criminals are in the most wanted list.
- **Scope:** First we would develop the app just for display and search and then we could divide into different categories of crimes.

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* User can see most-wanted list
* User can choose specific categories of most-wanted individuals, filtering usual stream down
* User can tap on the photo shown of an individual and be taken to a detail screen

### 2. Screen Archetypes

* Stream
   * User can view a basic most-wanted list

* Categories
   * User can choose from an array of categories, filtering the usual stream down to gender, location, type of crime, age, etc. 

* Detail
   * Tapping on an individual's picture pushes the user to a detail screen, providing a detailed description of this person's criminal profile
   
### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Home (stream)
* Categories
* Detail

**Flow Navigation** (Screen to Screen)

* Both categories and detail provide the option of navigating to the detail screen
   * Home => Detail
   
   * OR
   * Categories => Detail

## Wireframes
<img src="WireframeMWA.jpg" width=600>

### [BONUS] Digital Wireframes & Mockups
.
### [BONUS] Interactive Prototype

## Schema 
### Models
#### Main_Page
   | Property      | Type     | Description |
   | ------------- | -------- | ------------|
   | .criminalId   | String   | unique id for the criminal|
   | name          | String   | name criminal |
   | image         | String   | image of the criminal |
   | typeOfCrime   | String   | type of crime he/she is guilty |
   | warning       | Srting   | warning message |
  
### Networking
- Home screen 
  - (Read/Get) Query all criminals listed in the FBI website
- Criminal Profile
  - Complete profile of the criminal
- Search screen
  - Divide criminals into crime types
- Base URL: https://api.fbi.gov/wanted/v1/list

