# Simple Load Balancer

## Overview

This project implements a simple load balancer with the following features:
1. Round-robin and random selection load balancing algorithms.
2. Dynamic registration and removal of backend servers.
3. Error handling for failed requests.
4. Handling multiple concurrent requests efficiently.

## Setup Instructions

### Prerequisites

- Java 8 or later

### Running the Application

1. Clone the repository.
2. Navigate to the project directory.
3. Run the application using the Maven wrapper:
    ```bash
    ./mvnw spring-boot:run
    ```

### API Endpoints

- **Handle Request**: `/load-balancer/request?path=YOUR_PATH`
- **Add Server**: `/load-balancer/add-server?url=SERVER_URL`
- **Remove Server**: `/load-balancer/remove-server?url=SERVER_URL`
- **Set Strategy**: `/load-balancer/set-strategy?strategy=STRATEGY_NAME`

## Call Flow Diagrams

### High-Level Call Flow

```text
Client -> LoadBalancer -> BackendServer
```
