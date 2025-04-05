# Elastic Stack

This repository provides a simple and scalable way to deploy and manage the Elastic Stack components—Elasticsearch, Logstash, and Kibana—using Docker Compose. The Elastic Stack allows you to collect, analyze, and visualize data in real-time, making it a powerful tool for data analytics, logging, and monitoring.

## Components

- **Elasticsearch**: A distributed search and analytics engine, capable of storing and indexing large volumes of data.
- **Logstash**: A data processing pipeline that ingests, transforms, and sends data to Elasticsearch.
- **Kibana**: A browser-based analytics and visualization platform for interacting with Elasticsearch data.

## Features

- Easy setup with Docker Compose.
- Scalable for small to large environments.
- Real-time data analysis and visualization.
- Configurable for different use cases and environments.

## Prerequisites

- [Docker](https://www.docker.com/products/docker-desktop) and [Docker Compose](https://docs.docker.com/compose/) installed on your system.

## Getting Started

Follow these steps to get your Elastic Stack up and running:

### 1. Clone the Repository

First, clone this repository to your local machine:

```bash
git clone https://github.com/Strong-Foundation/elastic-stack.git
```

### 2. Navigate to the Project Directory

Change into the project directory:

```bash
cd elastic-stack
```

### 3. Start the Stack

Run the following command to start Elasticsearch, Logstash, and Kibana in the background using Docker Compose:

```bash
docker-compose up -d
```

This will start the services and run them in detached mode.

### 4. Access Kibana

Once the stack is up and running, you can access Kibana by navigating to `http://localhost:5601` in your web browser. Kibana provides an easy-to-use interface to query, visualize, and interact with your Elasticsearch data.

## Configuration

- **Elasticsearch Configuration**: You can modify the `docker-compose.yml` file to set environment variables and adjust settings for your Elasticsearch cluster.
- **Logstash Configuration**: The Logstash pipeline can be customized by editing the `logstash.conf` file, which allows you to define input sources, filters, and output destinations.

## Stopping the Stack

To stop the stack, run:

```bash
docker-compose down
```

This will stop all the services and remove the containers.

## Additional Resources

- [Elastic Stack Documentation](https://www.elastic.co/guide/index.html): Official documentation for Elasticsearch, Logstash, and Kibana.
- [Docker Compose Documentation](https://docs.docker.com/compose/): Documentation for understanding and using Docker Compose.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
