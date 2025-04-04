# Dwight - AI Content Moderation System

Dwight is a comprehensive solution for responsible and compliant use of Generative AI within organizations. It provides real-time monitoring, risk detection, and compliance enforcement for AI interactions.

## Features

- Real-time content moderation
- Sentiment analysis
- Entity recognition
- Compliance monitoring
- Risk scoring
- User authentication
- Audit logging
- Prometheus metrics
- Grafana dashboards

## Prerequisites

- Docker and Docker Compose
- Python 3.9+
- PostgreSQL
- Redis

## Installation

1. Clone the repository:
```bash
git clone https://github.com/your-org/dwight.git
cd dwight
```

2. Create a `.env` file based on `.env.example`:
```bash
cp .env.example .env
```

3. Update the environment variables in `.env` with your configuration.

4. Build and start the services:
```bash
docker-compose up --build
```

## API Documentation

Once the application is running, you can access the API documentation at:
- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

## Monitoring

- Prometheus: http://localhost:9090
- Grafana: http://localhost:3000 (default credentials: admin/admin)

## Development

1. Create a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the application:
```bash
uvicorn dwight.main:app --reload
```

## Testing

Run the test suite:
```bash
pytest
```

## Project Structure

```
dwight/
├── api/                # API endpoints
├── core/               # Core functionality
├── models/             # Database models
├── services/           # Business logic
├── utils/              # Utility functions
├── config/             # Configuration
├── tests/              # Test suite
└── main.py             # Application entry point
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Team

- Ayush Mati
- Manas Singh
- Priya Jha
- Prathmesh Shukla

# Problem Statement :
Create a solution for responsible and compliant use of Generative AI, focusing on OpenAI's ChatGPT within organizations. Design an automated system to monitor and prevent risks like inappropriate content, regulatory violations, and privacy breaches. Ensure real-time monitoring, risk-based alerts, and compliance with organizational policies and regulations. Aim for innovation, scalability, and ethical deployment to build trust among users and stakeholders.

# AI Implementation :
AI will be used to analyze user interactions with ChatGPT in real-time (Based on Microsoft-Azure), detect risks like inappropriate content, and assess their severity. Machine learning models will continuously learn and adapt to improve accuracy. Automated alerting mechanisms will notify personnel when risks are detected. Adaptive learning systems will refine monitoring rules based on feedback and regulatory changes, ensuring compliance and promoting responsible usage.

# NLP implementation :
For the NLP implementation in this project:
1. Real-time Analysis: Natural Language Processing (NLP) algorithms will analyze user interactions with ChatGPT in real-time.
2. *Sentiment and Intent Detection: NLP models will detect sentiment, intent, and context to assess the nature of each interaction.
3. Risk Identification: These algorithms will identify potential risks such as inappropriate language, sensitive topics, or regulatory violations.
4. Continuous Learning: The NLP system will continuously learn and adapt based on feedback and new data to improve accuracy over time.
5. Integration: NLP capabilities will be integrated into the automated monitoring system to enable real-time risk assessment of user interactions with ChatGPT.

# Conclusion:
In conclusion, this project ensures responsible use of ChatGPT through AI-powered monitoring, real-time risk detection, and compliance with regulations. With adaptive learning and adherence to policies, it fosters trust and innovation, laying a solid foundation for ethical AI deployment within organizational boundaries.

