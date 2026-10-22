<div align="center">

<img src="assets/banner.png" width="100%" alt="Akram Mujtaba, Data Engineer" />

<img src="https://readme-typing-svg.demolab.com?font=Inter&weight=600&size=19&pause=1400&color=38BDF8&center=true&vCenter=true&width=720&lines=Real-time+pipelines+with+Kafka%2C+Flink+and+Spark;Lakehouses+on+Iceberg%2C+Trino+and+AWS;Data+people+can+trust%2C+delivered+in+minutes" alt="Real-time pipelines, lakehouses, trusted data" />

<a href="mailto:akrammuj04@gmail.com"><img src="https://img.shields.io/badge/Email-akrammuj04%40gmail.com-0ea5e9?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<a href="https://www.linkedin.com/in/mujtabam04"><img src="https://img.shields.io/badge/LinkedIn-Connect-0a66c2?style=for-the-badge" alt="LinkedIn" /></a>
<img src="https://img.shields.io/badge/Open%20to-Data%20Engineering%20roles-34d399?style=for-the-badge" alt="Open to data engineering roles" />

</div>

---

### About me

I'm a data engineer with nearly 5 years of experience building batch and streaming pipelines. I currently work on pricing and host-analytics data at **Airbnb**, where I moved booking and search data from 3-hour batch loads to 15-minute streaming with Kafka, Flink, and Iceberg.

Before that I built the first AWS data lake and CDC pipelines at **RUNO**, a SaaS company in Hyderabad, taking reporting from next-day to about every 30 minutes. I hold an **MS in Computer Science from NJIT**.

📍 NJ/NYC area · open to hybrid, remote, or relocation · on STEM OPT through July 2028 (no sponsorship needed until then)

---

### Featured project

<a href="https://github.com/Akrammujtaba/reconstream">
  <img src="https://raw.githubusercontent.com/Akrammujtaba/reconstream/main/docs/images/overview.png" width="100%" alt="ReconStream: real-time payment reconciliation" />
</a>

**[ReconStream](https://github.com/Akrammujtaba/reconstream)** catches payment problems (double charges, missing payments, bad refunds) about 40 seconds after they happen, instead of at month-end close.

| What it does | How |
|---|---|
| Streams every booking change and payment event | Debezium CDC from Postgres, signed webhooks, Kafka |
| Matches bookings to money in near real time | Spark Structured Streaming with an event-time watermark |
| Keeps alerts honest | Late payments close their own alerts; redeliveries are never double counted |
| Stores everything queryable | Apache Iceberg (bronze, silver, gold), Trino, dbt finance marts |
| Proves it works | Injected 321 known faults: **all 321 caught, 0 false alarms, 40s median detection** |

The repo also documents two real problems I hit and fixed: batch time growing with table size, and a Spark session caching bug that silently stopped detection. → [Design decisions](https://github.com/Akrammujtaba/reconstream/blob/main/docs/design-decisions.md)

---

### Tech I work with

**Streaming & processing**
<br/>
<img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" alt="Apache Spark" />
<img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" alt="Apache Kafka" />
<img src="https://img.shields.io/badge/Apache%20Flink-E6526F?style=flat-square&logo=apacheflink&logoColor=white" alt="Apache Flink" />
<img src="https://img.shields.io/badge/Debezium%20CDC-91D443?style=flat-square" alt="Debezium CDC" />
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="SQL" />

**Lakehouse & warehouse**
<br/>
<img src="https://img.shields.io/badge/Apache%20Iceberg-3D7BBF?style=flat-square" alt="Apache Iceberg" />
<img src="https://img.shields.io/badge/Trino-DD00A1?style=flat-square&logo=trino&logoColor=white" alt="Trino" />
<img src="https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white" alt="dbt" />
<img src="https://img.shields.io/badge/Redshift-8C4FFF?style=flat-square" alt="Redshift" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
<img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" alt="MongoDB" />

**Orchestration, quality & cloud**
<br/>
<img src="https://img.shields.io/badge/Apache%20Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white" alt="Apache Airflow" />
<img src="https://img.shields.io/badge/Great%20Expectations-FF6310?style=flat-square" alt="Great Expectations" />
<img src="https://img.shields.io/badge/AWS%20(S3%2C%20EMR%2C%20Glue%2C%20MSK)-232F3E?style=flat-square" alt="AWS" />
<img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white" alt="Terraform" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions" />
<img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" alt="Grafana" />

---

### How I work

```text
Measure it, don't claim it    → every pipeline gets a way to prove it's correct
Idempotent by default         → any batch can be replayed without double counting
Event time over wall time     → late and out-of-order data is the normal case
Write down the why            → design decisions live next to the code
```

---

### Right now

- 🔧 Improving ReconStream weekly: see the [roadmap](https://github.com/Akrammujtaba/reconstream/blob/main/ROADMAP.md)
- 📚 Going deeper on Flink state management and Iceberg table maintenance at scale
- 💬 Happy to talk about streaming, CDC, and lakehouse design

