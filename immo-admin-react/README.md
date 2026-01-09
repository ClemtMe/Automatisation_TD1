# Immo admin client 

Simple admin client for Immo API using Vue 3

## Installation

- Create `.env` from `.env.exemple`
- Update environement variable
- Launch docker-compose

## Project Structure

```text
immo-admin-react/
├── .env.example       # Template for environment variables
├── .env               # Actual env file (gitignored)
├── docker-compose.yml # App container
├── Dockerfile         # Dockerfile for the React app
├── public/            # Public assets
├── src/               # Application source code
└── package.json      # Dependencies
```

## Usage
- Access the application at `http://localhost:3000`
- Make sure the immo API is running and accessible at the URL specified in the `.env` file.
```

