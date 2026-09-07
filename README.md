# Hi, I'm Devyanshu Sinha
**Computing Undergraduate @ Imperial College London**
I enjoy building things end-to-end and figuring out how systems actually work under the hood. Most of my projects sit somewhere between software engineering and data, and I like picking them apart until I understand every layer.
- **Currently exploring:** backend systems, data pipelines, and a bit of everything in between.
- **Education:** BEng Computing @ Imperial College London.
- **Let's connect:** reach out via email or LinkedIn below.
## Tech Stack
**Programming Languages:** Python, C++ / C, SQL, Haskell, Kotlin, Java.
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
![Kotlin](https://img.shields.io/badge/kotlin-%237F52FF.svg?style=for-the-badge&logo=kotlin&logoColor=white)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Haskell](https://img.shields.io/badge/Haskell-5e5086?style=for-the-badge&logo=haskell&logoColor=white)
**Systems & Data Libraries:** std::atomic, XGBoost, NumPy, Pandas, scikit-learn.
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
**Tools & Frameworks:** Spring Boot, CMake, Docker, FastAPI, PostgreSQL, Redis, Git, GitHub Actions.
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-%23008FBA.svg?style=for-the-badge&logo=cmake&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
## Featured Projects
### stream-processing-engine
> **A lock-free, multi-stage stream processing engine in C++20. Sustains ~96M events/sec across 12 cores with p50 1.4µs end-to-end latency, validated under TSan/ASan.**
A concurrent event pipeline built around a lock-free SPSC ring buffer, using acquire/release memory ordering and cache-line-aligned slots to avoid false sharing. Batched atomic publication amortises synchronisation cost across events, achieving a 20x throughput improvement over a mutex-guarded baseline. The pipeline itself runs three stages with bounded queues, backpressure propagation, and windowed aggregation for real-time rolling statistics.
### demand-forecasting-service
> **An end-to-end time-series forecasting service on real grid-demand data, with leakage-aware walk-forward validation and a production-shaped serving layer.**
A forecasting pipeline built on PJM hourly electricity demand data, with a feature layer generating lagged, rolling, and seasonal features under a strict no-lookahead discipline, backed by a test that proves it. Evaluated via chronological walk-forward validation against naive baselines, reducing RMSE by over 75%. Served behind a containerised FastAPI + Postgres + Redis stack sustaining ~339 req/sec with a 92% latency reduction from caching.
### task-scheduling-service
> **A distributed task scheduling service in Java and Spring Boot, with exactly-once job claiming across concurrent workers and an automated CI/CD pipeline.**
A backend job scheduler built around a PostgreSQL queue using row-level locking (SKIP LOCKED) so concurrent workers each claim disjoint work, with optimistic locking on status updates, a stale-job reaper to recover jobs orphaned by crashed workers, and exponential backoff on retries. Exposes a JWT-secured REST API sustaining ~835 enqueues/sec, tested with a Kotlin and JUnit suite against real PostgreSQL, and continuously built, tested, and published as a container image via GitHub Actions.
## Socials
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/devyanshusinha/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:devyanshusinha973@gmail.com)
