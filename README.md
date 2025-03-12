# **Data Pipeline with AWS and Apache Kafka**

## **Overview**
This project demonstrates a scalable data pipeline using AWS and Apache Kafka for real-time and batch data processing. It enables efficient data ingestion, transformation, storage, and querying.

## **Technologies Used**
- **Python**
- **AWS**: S3, Athena, Glue (Crawler & Catalog), EC2
- **Apache Kafka**: Real-time event streaming

## **Architecture**
1. **Data Sources** → Kafka Topics
2. **Kafka Consumer** → Stores data in S3
3. **AWS Glue** → Catalogs and transforms data
4. **AWS Athena** → Queries processed data
5. **AWS EC2** → Hosts pipeline processes

## **Features**
- Real-time data ingestion with Kafka
- Schema inference and transformation using Glue
- SQL-based querying via Athena
- Scalable and cost-efficient architecture

## **Setup**
1. **Clone Repository & Install Dependencies**
   ```bash
   git clone <repository_url>
   cd <project_directory>
   pip install -r requirements.txt
   ```
2. **Configure AWS Credentials**
   ```bash
   aws configure
   ```
3. **Start Kafka & Create Topics**
   ```bash
   kafka-server-start.sh <config_path>
   kafka-topics.sh --create --topic <topic_name> --bootstrap-server <broker>
   ```

## **Usage**
- **Run Producer:** `python kafka_producer.py`
- **Run Consumer:** `python kafka_consumer.py`
- **Process Data with AWS Glue**
- **Query Data using Athena**

## **Future Enhancements**
- Monitoring with CloudWatch/Prometheus
- Automate workflows with Apache Airflow

## **Contributors**
- Pragadeeswaran J

## **License**
Licensed under the [MIT License](LICENSE).

