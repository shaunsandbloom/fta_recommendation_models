# FTA TrAMS Recommendation System

## Background

The Federal Transit Administration is a federal transit program created under the The Urban Mass Transportation Act of 1964. Today, FTA administers a $20 billion annual program with the historic funding provided by the 2021 [Infrastructure Investment and Jobs Act](https://www.transit.dot.gov/iija). For more information on FTA's grant programs, please visit go [here](https://www.transit.dot.gov/grants)

The Transit Award Management System (TrAMS) is FTA's web-based grant management tool that allows recipients to apply for federal funds, manage their programs in accordance with federal requirements, and enable FTA to review, approve, control, and oversee how funds are used. For more information on TrAMS, please visit the [official website](https://www.transit.dot.gov/funding/grantee-resources/teamtrams/transit-award-management-system-trams).

## Introduction

The objective of the recommendation system is to assist grant recipients in choose appropriate budget activity line items (ALIs) when defining the scope of their projcet, reducing administrative activities, minimizing clerical errors, speeding up the grant award process.

This repository contains examples of how data are used to formulate recommendation models, calculate correlations in the relationships between ALI codes, as well as relationships between ALI codes and other features extracted from grant applications.

## Data Elements

In the sample set, each observation represents a single **grant award**. Below is a list of features found in each observations, which are used in varying algorithms to help measure similarity.

| Feature    | Description | Example |
| ---------- | ----------- | ------- |
| `awd_id`   | **Grant Award ID:** A unique identifier for each grant awarded by FTA | `AZ-2018-000` |
| `rec_id`   | **Recipient ID:** A unique identifier for grant recipients | `1635` |
| `rec_name` | **Recipient Name:** Formal name of the grant-receiving agency | `Arizona Department of Transportation` |
| `ali_code` | **Activity Line Item Code:** A unique identifier for each ALI in the FTA database | `30.09.01` |
| `ali_name` | **Activity Line Item Name:** A description of the ALI attached to the grant award | `Up to 50% FEDERAL SHARE` |
| `project_name` | **Project Name:** A description of the project grant funding would go toward | `2018 Formula Small Urban Funds (Capital, Operating and State Admin)` |


> [!IMPORTANT]
> This repository is purely for demonstration purposes and does not necessarily reflect the official policy or position of the Federal Transit Administration.
