# Semantic Web Crime Ontology

## Overview

The Semantic Web Crime Ontology is a structured knowledge representation system designed to model, analyze, and visualize crime-related data using semantic web technologies. This project focuses on crime data from the New York Police Department (NYPD) and the Los Angeles Police Department (LAPD), integrating ontology-driven data modeling, RDF conversion, and interactive visualization for advanced analytical insights.

## Implementation Details

### 1. Ontology Design and Enrichment

A comprehensive crime ontology has been developed using the Protégé platform to model crime-related entities accurately. The ontology defines structured classes, properties, and relationships to represent key aspects of crime incidents, including perpetrators, victims, locations, and temporal details. Domain-specific enrichments have been incorporated to ensure semantic precision and to support refined crime analysis.

### Knowledge Graph
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/56e748a6-dc9a-4436-b7f5-32fc3325ce42" />


### 2. Data Cleaning and Standardization

To maintain data integrity and consistency, extensive preprocessing was conducted using Python. The datasets from NYPD and LAPD were standardized through the following steps:

- Removal of non-essential columns
- Handling of missing values
- Standardization of time formats, age classifications, and racial demographics
- Addition of a 'holiday' attribute to track crimes occurring on public holidays

These steps ensure alignment with the ontology and facilitate seamless RDF transformation.

### 3. RDF Conversion

Following data refinement, the structured datasets were converted into RDF format using Protégé. The RDF transformation process ensures that tabular crime data is translated into meaningful RDF triples, capturing semantic relationships between crime-related entities. This conversion enables enhanced data interoperability and analytical capabilities.

### 4. Storing in GraphDB

GraphDB is employed as the triple store for managing and querying RDF data efficiently. The structured RDF data is ingested into GraphDB, allowing for optimized SPARQL querying. This setup ensures high-performance data storage, retrieval, and management, facilitating complex crime pattern analysis across NYPD and LAPD jurisdictions.

### GraphDB Representation
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/2ddd3a9e-ddb6-43ee-b92f-dc37cc866db8" />


### 5. Backend API Development with Node.js

A Node.js backend API has been developed to interface with the GraphDB triple store, enabling structured data retrieval through SPARQL queries. The API features:

- Well-defined endpoints for efficient access to crime data
- Robust querying mechanisms for advanced data analysis
- Comprehensive documentation to facilitate ease of use and system integration

### 6. Frontend Application using React.js

A web-based frontend application has been developed using React.js to provide an interactive platform for crime data exploration. The user interface includes:

- Dynamic data visualization through charts, graphs, and geospatial maps
- Intuitive navigation for analyzing predefined queries and crime trends
- Seamless integration with the backend API to ensure real-time data interaction

### UI Design
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/b6f2f850-01aa-4a46-a4b2-0685ce927ee2" />
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/98648544-6b08-4b57-9fe2-7fe8eaa706ee" />

# Instruction to Run Application Locally

## Prerequisites
- Ensure you have **Docker** installed on your device. Follow the installation guide [here](https://docs.docker.com/engine/install/).
- Run the **Docker Daemon** before proceeding.

## Installation & Setup

### Clone the Repository
```bash
git clone https://github.com/ssuryaw5/semantic-web-crime-ontology
cd semantic-web-crime-ontology
```

### Data Setup
1. Download the `data.zip` file from the provided canvas.
2. Extract and place the `data` folder inside the `semantic-web-crime-ontology` directory.

## Running the Application

### Start the Application
```bash
docker-compose -f docker-compose.services.yaml up
```

### Access the Application
Click the link below to test the application:
[Web Semantic Crime Analysis App](http://localhost:8080)

### Stop the Application
```bash
docker-compose -f docker-compose.services.yaml down
```


## Conclusion

The Semantic Web Crime Ontology leverages cutting-edge semantic web technologies to enhance crime data analysis in NYPD and LAPD jurisdictions. By integrating ontology-based data modeling, RDF transformation, and interactive visualization, this system provides a powerful tool for law enforcement agencies, policymakers, and researchers to derive actionable insights from crime patterns and trends.

